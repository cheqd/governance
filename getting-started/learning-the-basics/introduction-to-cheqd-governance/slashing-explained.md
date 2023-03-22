# Slashing explained

## How slashing works

The slashing module enables cheqd to disincentivize any attributable action by a protocol-recognized actor with value at stake by penalizing them ("**slashing**").

Penalties may include, but are not limited to:

* Burning some amount of their stake
* Removing their ability to vote on future blocks for a period of time.

Therefore, slashing should be an important consideration for both:

1. **Validators**; and
2. **Delegators**

We currently have the slashing values to:

1. **1% slashed** for downtime (getting jailed)
2. **5% slashed** for double signing

These values may change over time through proposals that are voted on the network.

## Delegator considerations

When delegating tokens to a validator in order to earn staking rewards, there is an obvious benefit in terms of the passive income that a delegator can receive. However, it is also very important for delegators to understand the potential risks of slashing.

Any tokens directly staked by the validator as well as delegated tokens are counted in what gets slashed for bad behaviour. This means that if a validator exhibits a double-sign infraction or downtime, you may be slashed:

* **1%** for (validator experiencing enough downtime to be put in validator jail).
* **5%** (for double-sign infraction)

For this reason, if you are delegated to a Validator and you notice them experiencing downtime, which can be seen on the [block explorer](https://explorer.cheqd.io/), it is suggested that you should **redelegate** your tokens to another Validator which is stable.

It is very important to note the difference between **redelegation** and **unbonding.** If you **redelegate** to another Validator within the 3 hour window before they are put in validator jail, you will likely escape any potential slashing. If you try and **unbond** your tokens from the Validator, since there is an unbonding period of **2 weeks,** you will still remain bound to the Validator in the short term and will experience a slash on your delegated tokens.

Understanding the difference between these two nuanced concepts is therefore important for any token holder that wants to bond, stake and delegate their tokens on the network.

## Validator considerations

### Tombstone Caps

In order to mitigate the impact of initially likely categories of non-malicious protocol faults, cheqd Network implements for each validator a _**tombstone**_ cap, which only allows a validator to be slashed once for a double sign fault.

For example, if you misconfigure your HSM and double-sign a bunch of old blocks, you'll only be punished for the first double-sign (and then immediately tombstombed). This will still be quite expensive and desirable to avoid, but tombstone caps somewhat blunt the economic impact of unintentional misconfiguration.

Liveness faults do not have caps, as they can't stack upon each other. Liveness bugs are "detected" as soon as the infraction occurs, and the validators are immediately put in jail, so it is not possible for them to commit multiple liveness faults without unjailing in between.

### Signing Info (Liveness)

Every block includes a set of precommits by the validators for the previous block, known as the `LastCommitInfo` provided by Tendermint. A `LastCommitInfo` is valid so long as it contains precommits from +2/3 of total voting power.

Proposers are incentivized to include precommits from all validators in the Tendermint `LastCommitInfo` by receiving additional fees proportional to the difference between the voting power included in the `LastCommitInfo` and +2/3.

Validators are penalized for failing to be included in the `LastCommitInfo` if they fail to sign **50% of the blocks** within the "signed\_blocks\_window". This window lasts for **25920 seconds** which equates to **7.2 hours**. As such, if the Validator exhibits downtime of roughly **3 hours**, it will be automatically jailed, potentially slashed, and unbonded.

Information about validator's liveness activity can be tracked through our block explorer:

{% embed url="https://explorer.cheqd.io/" %}
