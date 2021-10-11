# Primer on Tokenomics

Tokenomics are typically documented and distributed via a dedicated whitepaper. However, since a large proportion of the tokenomics for cheqd directly relate to governance and our tokenomics will be a constant iteration, it made most sense to incorporate them into the cheqd network’s [Governance Framework](https://docs.cheqd.io/governance/), which will also be continuously updated. We can then continue using [blogs](https://blog.cheqd.io) to explain the initial and updated tokenomics in an easier to digest format.

We have further assumed that readers are comfortable with concepts such as gas and block rewards and hence have not defined them here, but more info can be found in our [learning the basics page](https://docs.cheqd.io/governance/contributing/learning-the-basics). 

![cheqd Introducing Tokenomics image](<../.gitbook/assets/Introducing tokenomics.png>)

## Context <a href="3ef2" id="3ef2"></a>

Before diving into our tokenomics, it is first important to contextualise the project and our roadmap. Our overall aim is to establish payment rails for authentic data, including self-sovereign identity. Being able to share signed, verified and authentic data in a live environment has a myriad of benefits explained in our blog, [“Why SSI needs a Token”](https://blog.cheqd.io/why-self-sovereign-identity-needs-a-token-46e43dada01d)

![End-to-end payments where end clients do not need to worry about tokens / crypto](<../.gitbook/assets/cheqd end to end payments flow.png>)

An intermediate step will be transactional payments (i.e. payment for every Verifiable Credential), but core to our vision is the ability for ecosystems to create and maintain their own commercial models as we explained in the “[Business models of identity](https://blog.cheqd.io/the-business-models-of-identity-bb3336773727)”. Leveraging the analogy we used in the blog, this will establish:

* International trade rules -> Global payment layer: i.e. any entity (organisation or individual) can pay any other;
* Unilateral, bilateral, multilateral trade rules -> Ecosystems specific commercial models, i.e. any ecosystem can configure both governance and commercial models which establishes the incentives and structure it needs.

![cheqd’s transactional and ecosystem specific layers, allowing for anyone to interact with anyone, but also each ecosystem to set its own incentives](<../.gitbook/assets/cheqd tokenomic layers.png>)

So where does that leave us now? Putting this simply, the tokenomics below are what we are considering the Minimum Viable Tokenomics (“**MVT**”). Whilst these will establish a viable network, they are by no means the end-state and there is much, much more to come.

## Now <a href="b9ce" id="b9ce"></a>

Our first focus is launching a minimum viable network for authentic data. At a bare minimum, this means the ability to write and read identity ‘primitives’ (see below) to the network such that it can support the issuance and receipt of Verifiable Credentials (VCs) in a standards-based, interoperable fashion.

* DIDs: Decentralised identifiers
* Credential definitions
* Credential schemas

Therefore, whilst we have a tremendous roadmap we’re building to, the initial tokenomics will be simple.

## Incentives <a href="edf2" id="edf2"></a>

This section could go on forever since there is no end to the behaviour we want to either incentivise or dis-incentivise, and the behavioural economics and game theory which impacts this. To simplify drastically, we want to incentivise two main behaviours:

* Support for the network so that the fabric is maximally decentralised and resilient;
* Usage of the network for its intended purpose, i.e. authentic data transactions.

The reason for calling these out as a minimum is that they inform the network parameters we are about to discuss.
