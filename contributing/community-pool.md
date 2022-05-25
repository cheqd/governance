# Community Pool

cheqd will launch with community-spend capabilities, allowing CHEQ stakers to [Participants](../getting-started/learning-the-basics/introduction-to-cheqd-governance/what-is-bonding-delegation.md#what-is-a-participant) to approve spending from the Community Pool. **This documentation is in active development, so please seek feedback and take care when using this information.**

## Learn About the Community Pool

#### What is the balance of the Community Pool?

You can always see the balance of the cheqd Community Pools on one of our Block Explorers. Our main block explorer is here:

{% embed url="https://explorer.cheqd.io/" %}

Alternatively, you can use other block explorers found here:

{% embed url="https://learn.cheqd.io/getting-set-up-on-cheqd/block-explorers" %}

#### How can funds from the Community Pool be spent?

Funds from the cheqd Community Pool may be spent via successful governance proposal.

#### How should funds from the Community Pool be spent?

The prevailing assumption is that funds should be spent in a way that brings value to the cheqd Network. Or alternatively, something which benefits the wider world, such as spending the Pool on Carbon offset and sustainability.

#### How are funds disbursed after a community-spend proposal is passed?

If a community-spend proposal passes successfully, the number of $CHEQ encoded in the proposal will be transferred from the community pool to the address encoded in the proposal, and this will happen immediately after the voting period ends.

### Drafting a Community-spend Proposal

Drafting and submitting a proposal is a process that takes time, attention, and involves risk. The objective of this documentation is to make this process easier by preparing participants for what to pay attention to, the information that should be considered in a proposal, and how to reduce the risk of losing deposits. Ideally, a proposal should only fail to pass because the voters 1) are aware and engaged and 2) are able to make an informed decision to vote down the proposal.

If you are considering drafting a proposal, you should review the general background on drafting and submitting a proposal:

1. [How to contribute to cheqd;](https://gov.cheqd.io/contributing)
2. [How to draft a major network proposal and engage the community](https://gov.cheqd.io/contributing/major-network-changes)
3. [How voting on cheqd works](../getting-started/learning-the-basics/introduction-to-cheqd-governance/understanding-voting.md)

## Formatting a Community Pool Spend Proposal

There are five (5) components:

1. **Title** - the distinguishing name of the proposal, typically the way the that explorers list proposals
2. **Description** - the body of the proposal that further describes what is being proposed and details surrounding the proposal
3. **Recipient** - the cheqd address that will receive funding from the Community Pool
4. **Amount** - the amount of funding that the recipient will receive in nanoCHEQ (nCHEQ)
5. **Deposit** - the amount that will be contributed to the deposit (in nanoCHEQ ("nCHEQ") from the account submitting the proposal

**Off-ledger template**

You should use our forum for Community Spend Proposals to discuss the Proposal with the cheqd community:

{% embed url="https://commonwealth.im/cheqd" %}

#### On-ledger example

In this simple example (below), a network explorer will list the governance proposal as "Community Pool Spend." When an observer selects the proposal, they'll see the description. Not all explorers will show the recipient and amount, so ensure that you verify that the description aligns with the what the governance proposal is programmed to enact. If the description says that a certain address will receive a certain number of CHEQ, it should also be programmed to do that, but it's possible that that's not the case (accidentally or otherwise).

The `amount` is `1000000000ncheq`. 1 billion nano-cheq is equal to 1 CHEQ, so `recipient` address `cheqd1qgfdn8h6fkh0ekt4n4d2c93c5gz3cv5gce783m` will receive 1 CHEQ if this proposal is passed.

The `deposit 8000000000000 ncheq`results in 8000 CHEQ being used from the proposal submitter's account. There is a minimum deposit required for a proposal to enter the voting period, and anyone may contribute to this deposit within a 7-day period. If the minimum deposit isn't reach before this time, the deposit amounts will be burned. Deposit amounts will also be burned if quorum isn't met in the vote or if the proposal is vetoed.

```json
{
  "title": "Community Pool Spend",
  "description": "This is the summary of the key information about this proposal. Include the URL to a PDF version of your full proposal.",
  "recipient": "cheqd1qgfdn8h6fkh0ekt4n4d2c93c5gz3cv5gce783m",
  "amount": [
    {
      "denom": "ncheq",
      "amount": "10000000000000"
    }
  ],
  "deposit": [
    {
      "denom": "ncheq",
      "amount": "8000000000000"
    }
  ]
}
```

#### Real example in Cosmos Hub community

This is the governance proposal that [Gavin Birch](https://twitter.com/Ether\_Gavin) ([Figment Networks](https://figment.network)) used to create [Prop23, the first successful Cosmos Hub community-spend proposal](https://hubble.figment.network/cosmos/chains/cosmoshub-3/governance/proposals/23).
