# Validators and Node Operators

### What is a **Validator** or **Node Operator**?

In blockchain ecosystems, the **Node Operator** runs what is called a **node**. A node can be thought of like a power pylon in the physical world, which helps to distribute electricity around a wide network of users.

![https://www.nationalgrid.com/stories/energy-explained/everything-you-ever-wanted-know-about-electricity-pylons](<../.gitbook/assets/image (3) (1) (1).png>)

Without these pylons, electricity would be largely centralised in one location; the pylons help to distribute power to entire wide-scale populations. And if one pylon fails, the grid is set up to circumvent this pylon and re-route the electricity a different route.

Similarly, in blockchain infrastructure, each node runs an instance of the consensus protocol and helps to create a broad, robust network, with no single points of failure. A node failing will have little impact on the Network as a whole; however, if multiple nodes fail, or disagree with information entered into the transaction, then the block may not be signed, and there are fail-safe measures to notify the rest of the Node Operators of this.

The terms Validator and Node Operator are somewhat synonymous. Validator is the term used more commonly in the[ Cosmos documentation](https://docs.cosmos.network) when referring to a Node Operator that is validating transactions on a blockchain. The only point worth mentioning is you can have a Node Operator that is NOT a Validator. These are known as Observer nodes which play a more passive role on the network, as they don’t stake on the network or validate transactions, but can observe them.

### How do I set up a node?

If you are interested in creating a node to validate on cheqd, please refer to the Node Operator documentation here:

{% embed url="https://docs.cheqd.io/node" %}

### As a Validator, is my commission rate important?

As a Validator Node, you must set a rate of commission. This is the percentage of tokens that you take as a fee for running the infrastructure on the network. Token holders are able to delegate tokens to you, with an understanding that they can earn staking rewards, but as consideration, you are also able to earn a flat percentage fee of the rewards on the delegated stake they supply.

A **lower commission rate** = **higher likelihood** of **more token holders delegating** tokens to you because they will **earn more rewards**.

A **higher commission rate** = **you earn more tokens** from the existing stake + delegated tokens. But the tradeoff being that it **may appear less desirable for new delegators** when compared to other Validators.

You can have a look at other projects on Cosmos here to get an idea of the percentages that nodes set as commission.

{% hint style="info" %}
Please note, that once you set a maximum commission rate, **you are not able to change this going forward**. You will only be able to have a commission at that max or lower.
{% endhint %}

You also need to set a parameter called Commission Rate Max Change. This parameter sets the limit of which a commission rate can be changed within a single day. This helps protect those users who have delegated to Node Operators from delegating to a Node Operator with a low commission and it changing overnight. This parameter is also public, so a lower figure here is likely better if your goal as a Validator is to attract more users to delegate to you. We hope that you do your own research and make an informed decision on these parameters.

