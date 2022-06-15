# Understanding voting

## Understanding voting

Voting on cheqd is a core part of the Network and how each individual User can influence the direction of change. cheqd voting is based on a [liquid democracy](https://en.wikipedia.org/wiki/Liquid\_democracy) model, whereby Users can vote unilaterally or delegate their votes to a Node Operator of their choice.

If you already fully understand voting, you can go to our pages on staking, delegating and voting practically:

{% content-ref url="../../../contributing/how-do-i-stake-delegate-and-vote-practically.md" %}
[how-do-i-stake-delegate-and-vote-practically.md](../../../contributing/how-do-i-stake-delegate-and-vote-practically.md)
{% endcontent-ref %}

{% content-ref url="../../../contributing/how-do-i-vote-practically.md" %}
[how-do-i-vote-practically.md](../../../contributing/how-do-i-vote-practically.md)
{% endcontent-ref %}

Or you can jump straight into our Governance dashboard here:

{% embed url="https://cheqd.omniflix.co/" %}

### Users

Users are people, organisations or other entities that hold tokens.

### Participants

Participants are Users that have the right to vote on proposals. In the cheqd Network, Participants have tokens that are bonded and in the [active pool](what-is-the-active-pool.md).

1. Node Operators can '**stake'** their tokens in order to vote on governance matters. This initial stake, when added to the active pool, is also known as **bonded**;
2. Everyday Users can **‘delegate’** their tokens to a Node Operator, which then add to the amount **bonded** on that node.

{% hint style="info" %}
Unbonded CHEQ holders and other Users do not get the right to participate in voting on Proposals. However, they can submit and deposit on Proposals.
{% endhint %}

Some participants can be forbidden to vote on a proposal under a certain Node Operator if:

* Participant has bonded or unbonded CHEQ to a particular Node Operator after the proposal has entered its **voting period**.
* Participant set up a node and became a Node Operator after the proposal entered its **voting period**.

This does not prevent the participant voting with CHEQ bonded to another Node Operator. For example, if a participant bonded some CHEQ to Node Operator _'A'_ **before** a proposal entered voting period and other CHEQ to Node Operator _'B'_ **after** proposal entered voting period, only the vote under Node Operator _'B'_ will be forbidden.

### Inheritance

If a Participant does not vote, the Node Operator will vote on behalf of the Participant, using the tokens it has been **delegated**.

If the Participant votes before its delegated Node Operator, it’s vote will take precedence; the Node Operator will not inherit the Participant's vote.

If the Participant votes after its Node Operator, it will override its Node Operator vote with its own. If the Proposal is urgent, it is possible that the vote will close before Participant has a chance to react and override their Node Operator's vote.

### Voting period

Once a proposal reaches _**MinDeposit**_, it immediately enters Voting period. We define Voting period as the interval between the moment the vote opens and the moment the vote closes. Voting period should always be shorter than the Unbonding period to prevent double voting.

The initial value of the cheqd Voting period was **1 week**.

This has since been reduced to **5 days** to accelerate the process of releasing updates. &#x20;

### Unbonding period

Unbonding period is defined as the time to withdraw delegated tokens from a Node Operator to gain full access to these tokens in liquid form.

The initial value of the cheqd Unbonding period is **2 weeks**.

### Redelegation

It is **always possible** to change (redelegate) the Node Operator you are delegated to, with a minimal time delay, using the redelegation option.&#x20;

You are also able to delegate to multiple Node Operators at the same time.

### Option set

The option set of a proposal refers to the set of choices a participant can choose from when casting its vote.

The initial option set includes the following options:

```
Yes
No
NoWithVeto
Abstain
```

_**NoWithVeto**_ counts as _**No**_ but also adds a Veto vote. This is significant because a **33.34%** veto will **burn** the tokens in the _**ModuleAccount**_. This means that the tokens will be destroyed and put beyond use. For this reason, it is important that Participants make reference to cheqd's Principles before using the veto vote.

Abstain option allows voters to signal that they do not intend to vote in favor or against the proposal but accept the result of the vote.

### Weighted Votes

{% hint style="info" %}
Note: Weighted voting may not be available in the first iteration of the cheqd Network
{% endhint %}

Users casting a vote on a proposal have the option to split their votes into several voting options. For example, a User could use 70% of its voting power to vote Yes and 30% of its voting power to vote No.

Often, the entity owning a particular governance address might not be a single individual. For example, a company might have different stakeholders who want to vote differently, and so it makes sense to allow them to split their voting power. Currently, it is not possible for them to do "passthrough voting" and give their users voting rights over their tokens. However, with this system, exchanges can poll their users for voting preferences off-chain, and then vote on-chain proportionally to the results of the poll.

For a weighted vote to be valid, the options field must not contain duplicate vote options, and the sum of weights of all options must be equal to 1.

### Quorum

Quorum is defined as the minimum percentage of voting power that needs to be cast on a proposal for the result to be valid.

The quorum as a default setting is **33.34%**.

Going forward, more complex quorum mechanisms, such as [Adaptive Quorum Biasing](https://wiki.polkadot.network/docs/learn-governance) should be considered.

### Threshold

Threshold is defined as the minimum proportion of Yes votes (excluding Abstain votes) for the proposal to be accepted.

Initially, the threshold is set at **50%** with a possibility to veto if more than **33.34% of votes** (excluding Abstain votes) are _**NoWithVeto**_ votes. This means that proposals are accepted if the proportion of Yes votes (excluding Abstain votes) at the end of the voting period is superior to **50%** and if the proportion of _**NoWithVeto**_ votes is inferior to **33.34%** (excluding Abstain votes).

### Node Operator's punishment for non-voting

At present, Node Operators are not punished for failing to vote.

### Governance address

At launch, the Governance address will be the main Node Operator address generated at account creation. This address corresponds to a different PrivKey than the Tendermint PrivKey which is responsible for signing consensus messages. Node Operators thus do not have to sign governance transactions with the sensitive Tendermint PrivKey.

### **Burned deposits**

Deposits are burned when proposals:

1. **Expire** - deposits will be burned if the deposit period **(1 week)** ends before reaching the minimum deposit **(8000 CHEQ)**;
2. **Fail** **to reach quorum** - deposits will be burned for proposals that do not reach quorum within the **5 day** voting period, i.e. **33,34%** of all staked CHEQ must vote;
3. **Are vetoed** - deposits for proposals with **33.4%** of voting power backing the 'no-with-veto' option are also burned.

To learn more about when you should exercise the **veto** vote, refer to our [Second Foundational Principle, the Balancing Principle](../../../principles/foundational-principles.md#2.-the-balancing-principle).

## Software Upgrade

If proposals are of type _**SoftwareUpgradeProposal**_, then nodes need to upgrade their software to the new version that was voted. This process is divided into two steps:

```
Signal
Switch
```

### Signal

After a _**SoftwareUpgradeProposal**_ is accepted, Node Operators are expected to download and install the new version of the software while continuing to run the previous version. Once a Node Operator has downloaded and installed the upgrade, it will start signaling to the network that it is ready to switch by including the proposal's proposalID in its precommits.

{% hint style="info" %}
Note: There is only one signal slot per precommit. If several _**SoftwareUpgradeProposals**_ are accepted in a short timeframe, a pipeline will form and they will be implemented one after the other in the order that they were accepted.
{% endhint %}

### Switch

Once a block contains more than 2/3rd precommits where a common _**SoftwareUpgradeProposal**_ is signaled, all the nodes (including Node Operator nodes, non-validating full nodes and light-nodes) are expected to switch to the new version of the software.
