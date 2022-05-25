# Major Network changes

## Major Network Changes

These are changes that have a materially significant effect on the Network. Such changes SHOULD be made via a Proposal, following the steps in the decision tree diagram below.

Major Network changes include, but are not limited to:

* Materially significant Architecture Decisions (**ADs**), such as:
  * An additional feature to cheqd;
  * Removal of a feature of cheqd;
* Parameter changes for the Network;
* Community pool decisions;
* Materially significant changes to a cheqd Principle;
* Partnerships or connections to other infrastructure.

## Decision Tree

To help YOU understand how to make changes on the cheqd Network, the decision tree below visualises how changes should be carried out.

![Tree diagram showing when to use on-chain and off-chain governance](<../../.gitbook/assets/On-chain vs off-chain decision tree.jpg>)

## Proposals

One of the most important questions in this Governance Framework is explaining how any [User](../../getting-started/learning-the-basics/introduction-to-cheqd-governance/what-is-bonding-delegation.md#what-is-a-user) or [Participant](../../getting-started/learning-the-basics/introduction-to-cheqd-governance/what-is-bonding-delegation.md#what-is-a-participant) can make a proposal or voice their opinion on the Network.

There are two ways of doing this:

1. **Informal ‘off-chain’ proposal**
2. **Formal ‘on-chain’ proposal’**

These will be discussed in turn.

### Informal off-chain proposal

Rather than making a proposal directly to the Network, proposals SHOULD first be made off-chain.

Off-chain governance is vital for building a healthy and active governance community.

cheqd's off-chain forum is on Commonwealth:

{% embed url="https://commonwealth.im/cheqd" %}

You SHOULD gain feedback on you proposal on Commonwealth before posting any proposal to the cheqd mainnet. Off-chain proposals give the User proposing the Proposal can have more confidence that a Proposal will reach minimum deposit and be approved on-chain.

#### Your Idea

Before you make a Network Proposal, you should engage people (ideally experts) informally about your idea. You should consider:

* Does it make sense?
* Are there critical flaws?
* Does it need to be reconsidered?

Governance proposals potentially impact many stakeholders. Introduce your idea with known members of the community before investing resources into drafting a formal proposal. Don't let negative feedback dissuade you from exploring your idea if you think that it's still important.

If you know people who are very involved with cheqd, send them a private message with a concise overview of what you think will result from your idea or proposed changes.

You could ask a simple question or present an idea on our Commonwealth, for example:

1. cheqd [Proposal Discussion forum](https://commonwealth.im/cheqd/discussions/2%20-%20Proposal%20Discussion)

You may also want to rationalise your idea, or ask your question to the wider community, in:

1. [cheqd Telegram](https://t.me/cheqd)
2. [cheqd Discord](https://discord.gg/AxwbG9pCMM)
3. [cheqd Community Slack](https://join.slack.com/t/cheqd-community/shared\_invite/zt-toqyo7b7-2g9qDRjx3otd6529dTqeIA)

Engagement is likely to be critical to the success of a proposal. The degree to which you engage with the cheqd community should be relative to the potential impact that your proposal may have on the Network.

#### Confident with your idea?

Great! However, we still recommend that you introduce your idea with members of the community before investing resources into drafting a proposal on-ledger. At this point you should seek out and carefully consider critical feedback in order to protect yourself from [confirmation bias](https://en.wikipedia.org/wiki/Confirmation\_bias). This is the ideal time to see a critical flaw, because submitting a flawed proposal will waste resources.

### Drafting a Proposal

If you've considered feedback from broad perspectives and think that what you're doing is valuable and that your strategy should work, and you believe that others feel this way as well, it's likely worth drafting a proposal.

To make reading and reviewing your Proposal easier for the community, we have created a set of templates which any Proposal should follow here, [GitHub Issues Templates](https://github.com/cheqd/cheqd-node/issues).

Or if you would prefer to use another tool to write your Proposal, you can select a template from the list below.

1. [Text-based Proposal Template](text-based-proposal-template.md)
2. [Parameter Change Proposal Template](parameter-change-proposal-template.md)
3. [Software Upgrade Proposal Template](software-upgrade-proposal-template.md)
4. [Community Pool Proposal](community-pool-proposal-template.md)

Engage the community with your draft proposal

1. Post a draft of your proposal as a thread in [cheqd Proposal Discussion forum](https://commonwealth.im/cheqd/discussions/2%20-%20Proposal%20Discussion)
2. Post a link to the proposal in the [cheqd Discord Proposal channel](https://discord.gg/RAU3KfRR)
3. Directly engage key members of the community for feedback. These could be large contributors, those likely to be most impacted by the proposal, and entities with high stake-backing (eg. high-ranked Node Operators; large stakers).
4. Target members of the community in a semi-public way before bringing the draft to a full public audience.
5. Alert the community to the draft proposal via:
   * Twitter, tagging accounts such as the [cheqd account](https://twitter.com/cheqd\_io)
   * [cheqd Telegram](https://t.me/cheqd)
   * [cheqd Discord Proposal channel](https://discord.gg/RAU3KfRR)
   * [cheqd Community Slack](https://join.slack.com/t/cheqd-community/shared\_invite/zt-toqyo7b7-2g9qDRjx3otd6529dTqeIA)

## Formal on-chain proposal

Once you have sensibly tested your Proposal and bounced your ideas around the community, you are ready to submit a Proposal on-chain.

There are two ways to submit a Proposal on chain, a technical and a non-technical way.

### On-chain Governance using Commonwealth

You are able to connect the [cheqd Commonwealth forum](https://commonwealth.im/cheqd) to your [Keplr wallet](https://learn.cheqd.io/getting-set-up-on-cheqd/cheqd-supported-wallets/keplr-wallet).

Once you have connected your Keplr wallet, you can create an On-Chain proposal directly through the interface.

![How to create a new on-chain Proposal on Commonwealth](<../../.gitbook/assets/new on chain proposal.jpg>)

You will need a minimum amount of 8000 $CHEQ in order to make a Governance Proposal using Commonwealth. This is important to reduce spam Proposals on the Network.

Currently, on Commonwealth, there is only a Text-Based Proposal and a Community-Spend Proposal option. Parameter Changes and Software Upgrade proposals must be made through the Command Line Interface, below.

### JSON file for Command Line Interface Proposal

If you are using the [cheqd Command Line Interface](https://docs.cheqd.io/node/docs/cheqd-cli), you must follow the instructions below.

Prior to sending the transaction that submits your Proposal on-chain, you must create a JSON file. This file will contain the information that will be stored on-chain as the governance Proposal. Begin by creating a new text (.txt) file to enter this information. Use these best practices as a guide for the contents of your proposal. When you're done, save the file as a .json file. See the examples that follow to help format your proposal.

Each Proposal type is unique in how the .json should be formatted:

1. **TextProposal**: All the proposals that do not involve a modification of the source code go under this type. For example, an opinion poll would use a proposal of type _**TextProposal**_.
2. **SoftwareUpgradeProposal**: If accepted, Node Operators are expected to update their software in accordance with the proposal.
3. **CommunityPoolSpendProposal**: details a proposal for use of community funds, together with how many coins are proposed to be spent, and to which recipient account.
4. **ParameterChangeProposal**: defines a proposal to change one or more parameters. If accepted, the requested parameter change is updated automatically by the proposal handler upon conclusion of the voting period.
5. **CancelSoftwareUpgradeProposal**: is a gov Content type for cancelling a software upgrade.

To create a new Proposal type, you can propose a _**ParameterChangeProposal**_ with a custom handler, to perform another type of state change.

Once on-chain, most people will rely upon network explorers to interpret this information with a Graphical User Interface (GUI).

This is the command format for using cheqd’s CLI (Command-Line Interface) to submit your proposal on-chain:

```json
cheqd-noded tx gov submit-proposal \
  --title=<title> \
  --description=<description> \
  --type="TextProposal" \
  --deposit="8000000000000ncheq" \
  --from=<name> \
  --chain-id=<cheqd-mainnet-1>
```

### Proposal type

If \<proposal type> is left blank, the type will be a Text proposal. Otherwise, it can be set to _**param-change**_, _**community-pool-spend**_, _**software-upgdrade**_ or _**cancel-software-upgrade**_. Use _**--help**_ to get more info from the tool.

For instance, this is the complete command that I could use to submit a testnet parameter-change proposal right now:

```json
cheqd-noded tx gov submit-proposal \
--title=<Parameter change proposal> \
--description=<parameter change of min deposit> \
--type="param-change" \
--deposit="8000000000000ncheq" \
--from=<alex> \
--chain-id=<cheqd-mainnet-1>
--gas="auto"
--gas-adjustment"1.2"
--gas-prices="25ncheq"
```

1. cheqd noded is the [Command-Line Interface (CLI)](https://docs.cheqd.io/node/docs/cheqd-cli) client that is used to send transactions and query the cheqd testnet or mainnet;
2. tx gov submit-proposal and type='param-change' indicates that the transaction is submitting a parameter-change proposal;
3. \--from "alex" is the account key that pays the transaction fee and deposit amount;
4. \--gas the maximum amount of gas you accept may be used to process the transaction:
   * The more content there is in the description of your proposal, the more gas your transaction will consume;
   * If this number isn't high enough and there isn't enough gas to process your transaction, the transaction will fail;
   * The transaction will only use the amount of gas needed to process the transaction.
5. \--gas prices is a flat-rate incentive for a Node Operator to process your transaction:
   * The cheqd Network accepts zero fees, but many nodes will not transmit your transaction to the network without a minimum fee;
   * Many nodes use a minimum fee to disincentivize transaction spamming;
   * This can also be set to "auto"
6. \--gas-adjustment is the range of gas prices that will still enable the transaction to go through. We recommend "1.2"
7. \--the mainnet chain ID is **cheqd-mainnet-1**

{% hint style="info" %}
Note: be careful what you use for **--gas-prices**. A mistake here could result in spending hundreds or thousands of CHEQ accidentally, rather than ncheq, which cannot be recovered.
{% endhint %}

### Deposit

To prevent spam, Proposals must be submitted with a deposit in the coins defined in the _**MinDeposit**_ param. The voting period will not start until the Proposal's deposit equals _**MinDeposit**_.

When a Proposal is submitted, it has to be accompanied by a deposit that must be strictly positive, but can be inferior to _**MinDeposit**_. The submitter doesn't need to pay for the entire deposit on their own. If a Proposal's deposit is inferior to _**MinDeposit**_, other token holders can increase the Proposal's deposit by sending a Deposit transaction.

The deposit is kept in an escrow in the governance _**ModuleAccount**_ until the proposal is finalized (passed or rejected).

Once the proposal's deposit reaches _**MinDeposit**_, it enters the voting period. If a proposal's deposit does not reach _**MinDeposit**_ before _**MaxDepositPeriod**_, the proposal closes and nobody can deposit on it anymore.

In this scenario, the tokens spent on the Deposit which did not reach the _**MinDeposit**_ will be burnt, meaning that they will be removed from the active pool of tokens and put beyond use.

The **minimum deposit** for cheqd will initially be **8,000 CHEQ**.

The _**MaxDepositPeriod**_ will be **1 week**.

### Deposit refund and burn

When a proposal is finalized, the coins from the deposit are either refunded or burned, according to the final tally of the proposal:

* If a proposal does not reach _**MinDeposit,**_ the CHEQ in the governance _**ModuleAccount**_ will be burnt, which means that they will be put beyond use and removed from the ecosystem.
* If the proposal reaches _**MinDeposit**_ and is approved or rejected but not vetoed, deposits will **automatically be refunded to their respective depositor** (transferred from the governance _**ModuleAccount**_).
* If the proposal is approved, but the minimum quorum **(33.34%)** is not reached for the vote, deposits will be burned from the governance _**ModuleAccount.**_
* When the proposal is vetoed by **33.34%,** deposits will be burned from the governance _**ModuleAccount**_.

### Verifying your transaction

After posting your transaction, your command line interface will provide you with the transaction's hash, which you can query using the cheqd Block Explorer below:

{% embed url="https://explorer.cheqd.io/" %}

### Troubleshooting a failed transaction

There are a number of reasons why a transaction may fail. Here are two examples:

1. Running out of gas - The more data there is in a transaction, the more gas it will need to be processed. If you don't specify enough gas, the transaction will fail and your gas will be consumed by the network.
2. Incorrect denomination - You may have specified an amount in 'nanocheq' or 'microcheq' instead of 'ncheq', causing the transaction to fail.

If you encounter a problem, try to troubleshoot it first, and then ask for help. We also encourage you to propose edits to this document as the Network progresses so that it can improve for future use.
