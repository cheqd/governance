# Why should I delegate and stake my tokens?

**Participants** may be eligible for a percentage of the rewards that Node Operators earn during the course of running a node. Node Operators may offer a certain **commission** for delegating to them. Participants earn rewards on the delegated tokens which are bonded to the Validator.

Therefore, you may want to delegate and stake your tokens for two reasons:

1. To participate in Network Governance;
2. To earn rewards proportionate to your stake in the Network.&#x20;

### Network Governance

Users with **bonded** tokens, **Participants**, are able to vote on **Governance Proposals**. The weight of a vote is directly tied to the amount of bonded tokens delegated to Node Operators.

This is where the Delegated Proof of Stake system comes into play.&#x20;

1. If the User does not want to vote on a Governance Proposal or misses it for any particular reason, the Node Operator will **inherit** the **delegated** tokens and can use them to vote with.
2. If you are particularly interested or passionate about a specific governance proposal, or do not agree with your bonded Node Operator, it is absolutely possible to vote unilaterally. However, you must still have **delegated** tokens, **bonded** with a Node Operator to do so.&#x20;

To do this, follow the instructions in the section[ Voting on cheqd](https://docs.cheqd.io/governance/contributing/voting-on-cheqd).

In a nutshell:

**Node Operator voting power** = **initial stake** + **inherited delegated tokens** (if participants do not vote)

**Participant voting power** = **delegated tokens** (if participant chooses to vote)

### Network Rewards

#### 1. Block rewards

cheqd naturally has inflation, which means that it creates more blocks over time. Each time a new block is created, there is a chance that your Validator node will 'propose' that block (because it is in the validator pool). The higher the stake you hold, the higher this chance is. Over a period of time, by the law of averages, you will earn a reasonably consistent proportion of block rewards.

#### 2. Transaction fees

The more that DIDs are written to the Network (and in the future) verifiable credentials are verified by third parties, there will be transaction fees distributed to the network, which will be split between the Node Operators and those delegated to the Node Operators.

Gas prices also come into play here too, the lower your gas price, the more likely that your node will be considered in the active set for rewards.

You can read more about gas fees and prices here.

For context, we suggest the set gas-price should fall within this range: Low: 25ncheq Medium: 50ncheq High: 100ncheq

### How do I choose which **Node Operator** to **delegate** to?

Choosing your Node Operator or multiple Node Operators is an important decision. There a few things you can take into consideration:

1.  **Commission rate**

    The incentive for delegating tokens to a Node Operator, is that you, as a participant, can earn rewards based on the stake of the Node Operator. Each Node Operator will have a **commission rate.** This is the percentage of tokens that the Node Operator will take as **commission** for running the infrastructure - the remaining percentage is distributed to the **participants**.
2.  **Reputation**

    You should be mindful about what reputation the Node Operator has. This is because the Node Operator may use your votes against the best interest of yourself and the community. As cheqd evolves, it is likely that there will become a political spectrum of Node Operators, who will cast their vote in different directions. Some may want to create chaos on the network and vote to disrupt the established paradigms, for example. A chaotic actor may lure users to delegate to them with a favourable commission rate, and use the accumulated bonded tokens against the best interests of the network. For this reason the choice of Node Operator you delegate to is very important.
3.  **Slashing and Validator Jail**

    As the name would suggest, staking is not risk free. As the word stake literally means “having something to gain or lose by having a form of ownership of something”, individuals should be wary of the risk, as we’ll come on to.

    Think of it like this, if someone says to you “_what’s at stake_?” they are essentially asking: “_what am I risking in return for the potential rewards?_”

    Node Operators might exhibit bad behaviour on the Network and, as a result, have their stake slashed. Slashing means taking **stake** away from the Node Operator and adding it to the Community Pool.

Bad behaviour in this context usually means that the Node Operator has not signed a sufficient number of blocks as ‘pre commits’ over a certain period of time. This could be due to inactivity or potential malicious intent.

For example in June 2019, CosmosPool a former Cosmos validator, experienced a server outage on their main node; downtime that resulted in its validator being temporarily jailed and its stake being slashed by 0.01%, including that of its delegators. This was what’s call a downtime slashing incident (soft slashing) whereby the validator and delegators were punished for downtime proportionally to their stake on the network ([JohnnieCosmos](https://johnniecosmos.medium.com/what-you-need-to-know-when-staking-on-the-cosmos-ecosystem-e6fc13a1b0e3)). On top of this, further slashing later occurred as evidence was found of double block signing. Both CosmosPool AND the delegators’ stakes were slashed an additional 5% and the validator was peremandiet removed (‘tombstoned’).

Slashing can therefore certainly affect your delegated and bonded tokens, so it is important to consider your choice.

### What if I change my mind about a Node Operator? Is it possible to **redelegate** or **unbond** from a Node Operator?

Yes, it is possible to instantly **redelegate** to a new Node Operator; however, you cannot 'hop' between Node Operators quickly. You must complete your redelegation to a Node Operator before moving again. If you want to completely withdraw and **unbond** your tokens, you need to be mindful that this process takes **2 weeks** for the tokens to become available for use again. This **unbonding period** is an example of a parameter which can be adjusted by the Governance Framework process.
