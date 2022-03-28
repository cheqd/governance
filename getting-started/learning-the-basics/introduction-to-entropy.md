# ☄ Introduction to Entropy

## **Introduction** <a href="#76d0" id="76d0"></a>

The principle concept of **decentralised governance** is that no single person, entity or organisation can control the direction of change in a public Network. Instead, the direction of change is agreed by the democratic votes of an ever-growing, diverse collective.

This point is desirable to reach, because it maximises Network security and resilience, creates an environment which is governed by a broad, diverse and multijurisdictional collective, and enables the Network to function purely as a utility, regulating itself through its own [architecture](https://docs.cheqd.io/governance/getting-started/introduction-to-governance#4-architecture).

However, this point is not something that can be reached overnight. There is a transition period between the genesis event of any decentralised Network and the point at which sufficient decentralisation may be claimed.

We want cheqd to achieve sufficient decentralisation, and to dissolve the initial control over the Network that few stakeholders may have. We want decisions to be made by the Network, and not by ourselves, the initial core team.

This is why we have created the concept of **Entropy** to transparently and effectively achieve sufficient decentralisation, through **decentralised governance.**

## **Entropy** <a href="#fd67" id="fd67"></a>

Entropy is broadly defined as the degree of disorder or uncertainty in a system or process of degradation or a trend to disorder, according to the [Mirriam-Webster Dictionary](https://www.merriam-webster.com/dictionary/entropy). In Physics, and specifically, the Second Law of Thermodynamics, its function is best explained through a metaphor succinctly delivered by [Brian Cox](https://www.bbc.co.uk/programmes/p00fflcs).

Let’s think of a sandcastle sitting in a desert.

![Sandcastle stock image: https://jooinn.com/sand-castle.html](<../../.gitbook/assets/entropy sandcastle.png>)

The sandcastle in the desert has both order and structure, and there are very few ways to arrange the sand grains to achieve the same structure.

Nearly anything done to the sandcastle will remove some of the order and structure of the sandcastle, gradually eroding the sand away from the familiar and notable structure.

For this reason, the sandcastle can be said to have **Low Entropy** because it relies on order, structure and design.

Conversely, a pile of sand with roughly the same amount of sand grains as the sandcastle has immeasurably more ways of ordering the sand to look like a pile of sand. This is due to the relative disorder of the sand pile.

For this reason, the pile of sand, with many more ways to arrange it, has **High Entropy.**

Now imagine that the sandcastle was left in the desert all day. The winds in the desert would blow the sand around, and it would slowly disintegrate and fall to bits.

However, there is nothing fundamental in the laws of physics that says that the wind could not pick up some sand from a pile and deposit it in precisely, the exact shape of a sandcastle.

It is just extremely, extremely unlikely because there are very few ways of ordering the sand so it looks like a sandcastle.

It is overwhelmingly more likely that the wind will **take the Low Entropy structure**, the sandcastle, and **turn it into a High Entropy structure**, the sand pile.

In short, physics says that **Entropy always increases**.

This same pattern and natural law can be seen in the development of decentralised governance. And if modelled correctly, a decentralised Network can be created so that Entropy always increases, gradually making the Network more and more decentralised.

**The increasing of Entropy is one of cheqd’s foundational Principles, and we believe we can use it as a tool to achieve sufficient decentralisation efficiently and with transparency.**

## **The genesis event** <a href="#966f" id="966f"></a>

Like a perfectly formed sandcastle with Low Entropy, any decentralised ecosystem must begin with a structure, set of rules, parameters and default settings which govern the scope, boundaries and objectives of the Network — usually set by a small group of individuals.

For this reason every decentralised Network begins with a **Low Entropy genesis event** from which point Entropy increases.

This can be thought of like **a Big Bang**, starting a new system with a set of fundamental rules and boundaries.

Even the most high profile blockchains such as [Bitcoin](https://bitcoin.org) began with a notorious **‘genesis block**’. Also known as Block 0, the Bitcoin genesis block was the first block created on the Bitcoin ledger, and every single Bitcoin block can have its lineage and ancestry traced back to it.

Interestingly, the next block, known as Block 1, wasn’t mined until six days after the Genesis Block. This is considered as a very strange occurrence for the protocol, since the general time gap between blocks is intended to be \~10 minutes.

Many have questioned why Satoshi Nakamoto, the infamous pseudonymous creator of Bitcoin, caused the delay. The most likely theory is that Nakamoto spent the first 6 days testing the protocol and its stability, before backdating the timestamp.

Others believe that Nakamoto wanted to play God and recreate the story of the world being created in six days… Just like the Big Bang, Nakamoto had to create a set of default settings and parameters for Bitcoin to develop autonomously.

The point of this elaboration, however, is to highlight that for every Network that eventually reaches a point of sufficient decentralisation and High Entropy, there is a Big Bang event, and a period of tinkering and adjustment, as Low Entropy begins to increase.

And this is where we started at **cheqd**.

At its mainnet launch, cheqd defined a set of baseline conditions and [parameters](../../tokenomics/parameters/network-parameters.md) for the cheqd Network, using Cosmos’ inbuilt decentralised governance capabilities and [SDK](https://v1.cosmos.network/sdk).

Going forward, we want to clearly lay out how the Network will enable a smooth transition from a Low Entropy genesis event to a High Entropy, sufficiently decentralised structure.

## **How do we model Entropy?** <a href="#d1d6" id="d1d6"></a>

To model Entropy, we wanted to build more visual and accessible than an algorithm or formula; something that could be easily applied to multiple blockchains and utilised by any layperson and diverse audience .

**Where we landed was: a Scorecard**

![cheqd Entropy Scorecard](<../../.gitbook/assets/Entropy radar diagram blank.png>)

The spider diagram above, the Entropy Scorecard, shows a scale scoring from **1 - 5** which we refer to as Entropy Levels, measuring tangible decentralisation from a genesis state (and Low Entropy) to beyond the point of sufficient decentralisation (and High Entropy).

At each point on the diagram sits a different metric of measurement. It is important to note that we could have selected more, fewer or different metrics to calculate Entropy against. We chose the seven metrics listed below because they provide a very sensible, digestible foundation for a rough calculation of cheqd’s Entropy. These metrics cover each angle of the Network, from **security** to **geography** to **utility** to **governance**.

We would absolutely welcome suggestions and feedback from the community to further refine this list going forward. Get in touch with us using our [Governance discussion forum here](https://github.com/cheqd/cheqd-governance/discussions).

We will walk through our reasoning behind each choice:

1. **Validators (number)**

This is the number of Node Operators on the Network. This is significant because the composition of Node Operators on the Network has a direct relationship with the dilution of voting power. The greater the number of Node Operators, the:

1. Greater choice the token holders have in who to bond and delegate tokens to for the purpose of Network Governance.
2. Greater the strength of security on the Network, with fewer points of failure.

2\. **Developers (commits)**

This is the number of commits made on the source code after launch via cheqd’s open source repositories. Ideally, we would also be able to measure the amount of commits made by developers outside the core team of cheqd. Commits from developers outside cheqd add healthy randomness to the code and the development of the Network.

3\. **Participants (number)**

This is the number of bonded token holders, meaning the Network Users who have bound a portion of their tokens to a Node Operator in order to participate in Governance.\
\
This is important because the larger the pool of Participants, the more the voting power will become diluted across the Network, since Participants are able to vote unilaterally, regardless of the Node Operator they are bonded to.

4\. **Nakamoto coefficient (number)**

Taken from previous work done on blockchain decentralisation, this is the minimum number of Entities in the Network that can pool together to reach 51% stake on the Network. The higher the number here, the more the Network is secure against malicious attacks and undesirable breaking changes.

5\. **Exchanges (volume)**

Exchanges are closely correlated with the accessibility of the token. Being able to buy and sell CHEQ on an exchange will open the token up to a larger range of Users. A higher number of exchanges will lead to a healthier split of stake, with hypothetically, lower volume across each exchange.

6\. **Nodes (country)**

The geographical makeup of the Network is important when discussing decentralisation. This is because geographic diversity lends itself to diversity of thought and perspective. Furthermore, a geographically diverse Network increases the security because even if an entire country was to shut its infrastructure down, a multijurisdictional Network would continue resolutely.

7\. **Proposals (number)**

Like developer commits, Network Governance Proposals transition the Network away from its genesis state to a more random and disordered Entity. This again is very important in removing the initial control and order that the cheqd core team has implemented into the genesis state of the Network.

The Proposal and Voting process on cheqd is based on a liquid democracy. As a result, the more decisions are made through this process, the more control is taken away from a centralised collective and moved to the consensus of a wide-barrelled and diverse group of Participants.

### Calculating Entropy

Having laid out the distinct metrics used to constitute Entropy, it is next important to lay out the values that define each Entropy Level. These values are specific to cheqd and the levels of decentralisation we would like to eventually reach.

These values have been calculated by us looking at our end-goal, taking the point at which we feel we could be maximully or sufficiently decentralised, and scaling backwards.

The values that we have chosen are as follows:

| **Variable**                                                                | **Entropy Level 1** | **Entropy Level 2** | **Entropy Level 3** | **Entropy Level 4** | **Entropy Level 5** |
| --------------------------------------------------------------------------- | ------------------- | ------------------- | ------------------- | ------------------- | ------------------- |
| **Number of Node Operators (Validators)**                                   | 5                   | 10                  | 25                  | 50                  | 100                 |
| **Number of commits from outside core team**                                | 5                   | 10                  | 25                  | 50                  | 100                 |
| **Number of distinct Participants with bonded tokens**                      | 100                 | 500                 | 1000                | 5000                | 10,000              |
| **Number of stakeholders to achieve 51% of Network (Nakamoto coefficient)** | 2                   | 4                   | 8                   | 15                  | 30                  |
| **Exchanges (CEX and DEX) supported**                                       | 1                   | 2                   | 4                   | 6                   | 8                   |
| **Country distribution of node operators**                                  | 5                   | 10                  | 20                  | 40                  | 60                  |
| **Number of accepted Proposals after genesis**                              | 5                   | 10                  | 20                  | 40                  | 60                  |

To ‘score’ Entropy, you need to add the total sum of the Entropy Level across each metric.

For example, the highest level of decentralisation a Network could reach according to this model would be Entropy Level 5 in all metrics - totalling a score of **35**. Whilst the lowest level a Network could have would be Entropy Level 1 in all metrics - totalling a score of **5**.

We would also love to see other Networks applying the same scorecard model of Entropy to exhibit their Network’s level of decentralisation, and whilst slight changes may need to be made to accommodate for nuances in different Networks, the core concept can remain the same.

Over time, we do expect this initial table to be iterated, extended and revised as decentralised ecosystems in general become more mature, more distinct and as opinion from Regulators, such as the Security and Exchange Commission (SEC) becomes more clear.\\

### Entropy Progression

In this section we want to explain where we are, where we want to get to, and why we want to get there.

#### Where we started

Like any other blockchain Network, cheqd began its life cycle with a Low Entropy score. This is absolutely normal for the genesis of a decentralised Network, as the core team will have put in the default parameters, meaning there will be a higher locus of control, and change has not yet been made via the governance framework processes.

At launch our Entropy score was **lower than 14.**

A low entropy score as such, can be represented by the scorecard below:

![cheqd Low Entropy](<../../.gitbook/assets/Radar entropy low 2.png>)

This score quickly began to shift after launch as more participants joined from different geographies and stake began to spread more evenly. We will soon be launching a Governance Dashboard which shows where the network is on this scale.

#### Where we want to get to

We are aiming for high Entropy for various reasons, because it:

1. **Correlates with higher Network security and resiliency across countries;**
2. **Means broader contributions to the Network from a multidisciplinary and diverse collective;**
3. **Enables increased integration capabilities with other technologies to improve the ecosystem as a whole;**
4. **Increases the democratisation of wealth and dilution of rewards across a larger scope of actors;**
5. **Dilutes the control from a select group of people, to a genuinely decentralised and diverse collective.**

As a benchmark, we want to aim for an **Entropy Score** **greater than 28**; and with **none of the scores below Entropy Level 3.**

This combination is important because it will ensure that there is limited surface area for centralisation or control, as all metrics have progressed beyond a Low Entropy state.

A High Entropy Network would generate a scorecard illustrated by the example below:

![cheqd High Entropy](<../../.gitbook/assets/Entropy radar diagram - high entropy.png>)

At this point of High Entropy, we would hope that we would be considered a Network which is sufficiently decentralised, although of course this is not up for us to decide. Yet, we believe that this progression of Low to High Entropy is an important journey for every decentralised Network to embark on.

#### How do we plan to get there?

To increase Entropy, we have developed a governance framework that champions decentralisation as time progresses.

Achieving high Entropy involves:

1. **Making it easy for Node Operators to onboard in an Open Source way;**
2. **Having clear and transparent documentation, in multiple languages;**
3. **Having simple governance processes to evolve the Network baked into the protocol;**
4. **Incentivising a healthy community, with places to discuss positive and constructive ideas.**
5. **Enabling all parties to be remunerated for their active contribution and participation.**

And a combination of the above will increase the Network Entropy in a healthy and natural way, bridging the middleground between Low and High Entropy, as seen below:

![cheqd Entropy Overlapped](<../../.gitbook/assets/radar entropy overlap 2.png>)

As the initial team, we have a responsibility to, as we like to put it, create the first domino and push it over. Or in other terms, we need to take care in setting a strong technical foundation alongside a culture of transparency, inclusivity and open communication to push Entropy in the right direction.

### Where does this leave us?

Over the course of this series of blogs, we have introduced and explained the following:

1. Why decentralisation is an important goal for healthy blockchain Networks;
2. Why Increasing Entropy is crucial to achieving this goal;
3. How to model Entropy to achieve greater clarity.

And looking back now, what we want the reader to take away from this is to understand the following:

Decentralised Networks and protocols often leave a lot to be desired, especially when it comes to clearly defined lines.

Through our model of Entropy, we incentivise healthy behaviour, high resiliency, utility and generativity which should be the building blocks for any decentralised Network.

We also want this to move decentralisation towards greater regulatory clarity, rather than towards greater dissonance.

If we want to make self-sovereign identity, rooted on a decentralised Network a reality, we can only do this through being open, creative and inclusive in the way we work. Helping frame decentralised ecosystems in a way which makes sense for laypersons will bolster the chances of SSI and token payment rails being used in regulated industries worldwide.

The model of Increasing Entropy, as one of [cheqd’s Foundational Principles](https://docs.cheqd.io/governance/principles/foundational-principles), attempts to build greater clarity around the labelling and framing of decentralised ecosystems and DAOs. We hope the community can iterate and build on the work done here and respond with feedback and opinion. This eventually can create an even more robust framework and help make cheqd’s vision of a Web 3.0, the new paradigm for human interaction.
