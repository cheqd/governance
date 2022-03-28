# Staking

### What does **staking** mean?

**Stake** is the amount of tokens a **Node Operator** puts aside and dedicates to a network’s active pool, in order to contribute to governance and earn rewards. **Staking** is the verb used to describe this contribution. As cheqd is a Proof of Stake (PoS) Network, rewards can be earnt in direct correlation with the amount of stake a Node Operator contributes. Tokens which are in the active pool are known as ‘bonded’ tokens.

The goal for bonded tokens on the Network is **60%**. Below **60%** bonded tokens, the rate of inflation will increase, tending to **4%** **(inflation max)**. Above **60%** bonded tokens, the rate of inflation will decrease, tending towards **1% (inflation min)**.

When you setup your Validator node, you also need to set a minimum self-delegation which is the minimum amount of tokens you promise to keep bonded. This can be as low as 1 ncheq.

You can earn rewards proportionate to your stake in the Network. These include:

#### 1. Block rewards

cheqd naturally has inflation, which means that it creates more blocks over time. Each time a new block is created, there is a chance that your Validator node will 'propose' that block (because it is in the validator pool). The higher the stake you hold, the higher this chance is. Over a period of time, by the law of averages, you will earn a reasonably consistent proportion of block rewards.

#### 2. Transaction fees

The more that DIDs are written to the Network (and in the future) verifiable credentials are verified by third parties, there will be transaction fees distributed to the network, which will be split between the Node Operators and those delegated to the Node Operators.

Gas prices also come into play here too, the lower your gas price, the more likely that your node will be considered in the active set for rewards.

You can read more about gas fees and prices here.

For context, we suggest the set gas-price should fall within this range: Low: 25ncheq Medium: 50ncheq High: 100ncheq



### What does a **Validator** actually do?

The [Cosmos Hub](https://hub.cosmos.network/main/gaia-tutorials/what-is-gaia.html) is based on [Tendermint](https://tendermint.com/docs/introduction/what-is-tendermint.html), which relies on a set of validators to secure the network. By ‘secure the network’ this refers to the way in which validators “_participate in consensus by broadcasting votes which contain_ [_cryptographic signatures signed by their private key_](https://hub.cosmos.network/main/validators/validator-faq.html)”.

A cryptographic signature is a mathematical scheme for verifying the authenticity of digital messages or documents. A private key is like a password — a string of letters and numbers — that allows you to access and manage your crypto funds (your mnemonic is a version of this). So, the above is saying validators can broadcast that they agree with transactions in a block, using their password to sign their agreement in a mathematical way which ensures security and privacy.

### Can **Participants** earn tokens?

In short, yes. **Participants** may be eligible for a percentage of the rewards that Node Operators earn during the course of running a node. Node Operators may offer a certain **commission** for delegating to them. Participants earn rewards on the delegated tokens which are bonded to the Validator.

###

###
