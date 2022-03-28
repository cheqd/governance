# Validators and Node Operators

### What is a **Validator** or **Node Operator**?

In blockchain ecosystems, the **Node Operator** runs what is called a **node**. A node can be thought of like a power pylon in the physical world, which helps to distribute electricity around a wide network of users.

![https://www.nationalgrid.com/stories/energy-explained/everything-you-ever-wanted-know-about-electricity-pylons](<../.gitbook/assets/image (3) (1) (1).png>)

Without these pylons, electricity would be largely centralised in one location; the pylons help to distribute power to entire wide-scale populations. And if one pylon fails, the grid is set up to circumvent this pylon and re-route the electricity a different route.

Similarly, in blockchain infrastructure, each node runs an instance of the consensus protocol and helps to create a broad, robust network, with no single points of failure. A node failing will have little impact on the Network as a whole; however, if multiple nodes fail, or disagree with information entered into the transaction, then the block may not be signed, and there are fail-safe measures to notify the rest of the Node Operators of this.

The terms Validator and Node Operator are somewhat synonymous. Validator is the term used more commonly in the[ Cosmos documentation](https://docs.cosmos.network) when referring to a Node Operator that is validating transactions on a blockchain. The only point worth mentioning is you can have a Node Operator that is NOT a Validator. These are known as Observer nodes which play a more passive role on the network, as they don’t stake on the network or validate transactions, but can observe them.

### As a Validator, is my commission rate important?

As a Validator Node, you must set a rate of commission. This is the percentage of tokens that you take as a fee for running the infrastructure on the network. Token holders are able to delegate tokens to you, with an understanding that they can earn staking rewards, but as consideration, you are also able to earn a flat percentage fee of the rewards on the delegated stake they supply.

A **lower commission rate** = **higher likelihood** of **more token holders delegating** tokens to you because they will **earn more rewards**.

A **higher commission rate** = **you earn more tokens** from the existing stake + delegated tokens. But the tradeoff being that it **may appear less desirable for new delegators** when compared to other Validators.

You can have a look at other projects on Cosmos here to get an idea of the percentages that nodes set as commission.

Please note, that once you set a maximum commission rate, **you are not able to change this going forward**. You will only be able to have a commission at that max or lower.

You also need to set a parameter called Commission Rate Max Change. This parameter sets the limit of which a commission rate can be changed within a single day. This helps protect those users who have delegated to Node Operators from delegating to a Node Operator with a low commission and it changing overnight. This parameter is also public, so a lower figure here is likely better if your goal as a Validator is to attract more users to delegate to you. We hope that you do your own research and make an informed decision on these parameters.

### How do I choose which **Node Operator** to **delegate** to?

Choosing your Node Operator or multiple Node Operators is an important decision. There a few things you can take into consideration:

1.  **Commission rate**

    The incentive for delegating tokens to a Node Operator, is that you, as a participant, can earn rewards based on the stake of the Node Operator. Each Node Operator will have a **commission rate.** This is the percentage of tokens that the Node Operator will take as **commission** for running the infrastructure - the remaining percentage is distributed to the **participants**.
2.  **Reputation**

    You should be mindful about what reputation the Node Operator has. This is because the Node Operator may use your votes against the best interest of yourself and the community. As cheqd evolves, it is likely that there will become a political spectrum of Node Operators, who will cast their vote in different directions. Some may want to create chaos on the network and vote to disrupt the established paradigms, for example. A chaotic actor may lure users to delegate to them with a favourable commission rate, and use the accumulated bonded tokens against the best interests of the network. For this reason the choice of Node Operator you delegate to is very important.
3.  **Slashing and Validator Jail**

    As the name would suggest, staking is not risk free. As the word stake literally means “having something to gain or lose by having a form of ownership of something”, individuals should be wary of the risk, as we’ll come on to.

    Think of it like this, if someone says to you “_what’s at stake_?” they are essentially asking: “_what am I risking in return for the potential rewards?_”

    Node Operators might exhibit bad behaviour on the Network and, as a result, have their stake slashed. Slashing means taking **stake** away from the Node Operator and adding it to the Community Pool.\
    \
    Bad behaviour in this context usually means that the Node Operator has not signed a sufficient number of blocks as ‘pre commits’ over a certain period of time. This could be due to inactivity or potential malicious intent.

    For example in June 2019, CosmosPool a former Cosmos validator, experienced a server outage on their main node; downtime that resulted in its validator being temporarily jailed and its stake being slashed by 0.01%, including that of its delegators. This was what’s call a downtime slashing incident (soft slashing) whereby the validator and delegators were punished for downtime proportionally to their stake on the network ([JohnnieCosmos](https://johnniecosmos.medium.com/what-you-need-to-know-when-staking-on-the-cosmos-ecosystem-e6fc13a1b0e3)). On top of this, further slashing later occurred as evidence was found of double block signing. Both CosmosPool AND the delegators’ stakes were slashed an additional 5% and the validator was peremandiet removed (‘tombstoned’).

    Slashing can therefore certainly affect your delegated and bonded tokens, so it is important to consider your choice.

### What if I change my mind about a Node Operator? Is it possible to **redelegate** or **unbond** from a Node Operator?

Yes, it is possible to instantly **redelegate** to a new Node Operator; however, you cannot 'hop' between Node Operators quickly. You must complete your redelegation to a Node Operator before moving again. If you want to completely withdraw and **unbond** your tokens, you need to be mindful that this process takes **2 weeks** for the tokens to become available for use again. This **unbonding period** is an example of a parameter which can be adjusted by the Governance Framework process.
