# Why should I delegate and stake my tokens?

## Why should I delegate and stake my tokens?

****[Participants](delegation-and-bonding.md#what-is-a-participant) may be eligible for a percentage of the rewards that [Node Operators](validators.md#what-is-a-validator-or-node-operator) earn during the course of running a node. [Node Operators](validators.md#what-is-a-validator-or-node-operator) may offer a certain **commission** for delegating to them. Participants earn rewards on the delegated tokens which are bonded to the Validator.

Therefore, you may want to delegate and stake your tokens for two reasons:

1. To participate in Network Governance;
2. To earn rewards proportionate to your stake in the Network.

### Network Governance

Users with **bonded** tokens, [Participants](delegation-and-bonding.md#what-is-a-participant), are able to vote on **Governance Proposals**. The weight of a vote is directly tied to the amount of bonded tokens delegated to Node Operators.

This is where the Delegated Proof of Stake system comes into play.

1. If the User does not want to vote on a Governance Proposal or misses it for any particular reason, the Node Operator will **inherit** the **delegated** tokens and can use them to vote with.
2. If you are particularly interested or passionate about a specific governance proposal, or do not agree with your bonded Node Operator, it is absolutely possible to vote unilaterally. However, you must still have **delegated** tokens, **bonded** with a Node Operator to do so.

To do this, follow the instructions in the section [How do I vote practically?](../../../contributing/voting.md)

In a nutshell:

**Node Operator voting power** = **initial stake** + **inherited delegated tokens** (if participants do not vote)

**Participant voting power** = **delegated tokens** (if participant chooses to vote)

### Network Rewards

Users and Node Operators may also be interested in earning rewards for adding their tokens to the [active pool](active-pool.md). These rewards come in the form of:

#### 1. Block rewards

cheqd naturally has inflation, which means that it creates more blocks over time. Each time a new block is created, there is a chance that your Validator node will 'propose' that block (because it is in the validator pool). The higher the stake you hold, the higher this chance is. Over a period of time, by the law of averages, you will earn a reasonably consistent proportion of block rewards.

#### 2. Transaction fees

The more that DIDs are written to the Network (and in the future) Verifiable Credentials are verified by third parties, there will be transaction fees distributed to the network, which will be split between the Node Operators and those delegated to the Node Operators.

Gas prices also come into play here too, the lower your gas price, the more likely that your node will be considered in the active set for rewards.

For context, we suggest the set gas-price should fall within this range: Low: 25ncheq Medium: 50ncheq High: 100ncheq
