# Technical Standards & Interop

This document is specifically targeted towards SSI vendors and enthusiasts who want to understand what technical standards cheqd supports and intends to support going forward. 

Before diving into the standards themselves, it is important to highlight that we at cheqd want to bring the SSI community together. The way to achieve this is by being open, working alongside the community, and setting aside commercial interests for the progression of the industry as a whole.  

## The Network of Networks Issue

Part of the issue slowing the development of the SSI community as a whole is the Network-of-Networks issue.

**What does this mean?**

It means that a Verifiable Credential signed by a public DID routed on one Public Utility cannot be easily resolved by a wallet that does not natively support that Public Utility.

Let's take an easy example. Say I receive a Credential with a DID anchored on cheqd and present this to _Verifier A_.

If _Verifier A_ only supports, for example, Sovrin, DID web and Ethereum, then they will not be able to natively verify the Credential that I present. 

They would have to verify the Credential by using a Universal Resolver. 

The root cause of this issue is because in the W3C DID spec, there is no field that 'names' the particular Utility the DID is anchored to. For this reason, there is no native reference point for _Verifier A_ to know where to resolve the DID.

A [Network-of-Networks](https://networkofnetworks.net/wp-content/uploads/2021/05/EBSI_Network-of-Networks_esatus_Danube_Tech_TNO.pdf) is a proposed solution to this issue by the [European Self-Sovereign Identity Consortium \(ESSIC\)](https://networkofnetworks.net/wp-content/uploads/2021/05/EBSI_Network-of-Networks_esatus_Danube_Tech_TNO.pdf).

cheqd intends to engage the consortium and closely follow the movements here in order to reach a more interoperable DID ecosystem in the long term.

### Cosmos and Network-of-Networks

Part of our design choice for building on the Cosmos SDK was its work in the Network-of-Networks issue for tokens. 

In a similar vein to with DIDs, tokens issued on one Utility are generally only able to be consumed by software which supports the Utility. 

Cosmos' core ethos is to avoid this, and to bridge tokens across multiple ledgers. It has done this through the [Inter-Blockchain Communication Protocol \(IBC\). ](https://docs.cosmos.network/master/ibc/overview.html)

Conceptually the work to bridge ledgers in the token world is very similar to bridging the use of DIDs in the identity world. For this reason, we believe cheqd is well placed to help facilitate this movement towards interoperability. 

### cheqd position

We hear you: supporting cheqd and anchoring DIDs on cheqd does not yet solve the Network-of-Networks issue. And yes... ugh, another DID method is not helping anyone. 

But we do believe that cheqd is best placed to host identity primatives now, and when the Network-of-Network issue is resolved because of: 

1. **High Decentralisation**  
  
   Unlike other ledgers geared for hosting identity primatives, such as Hyperledger Indy or Sovrin, cheqd is vastly more decentralised via a liquid democracy governance model, explained throughout this Governance Framework.   


   This means that there is no centralised governance authority, but rather decisions are made by Network, wide-barreled consensus via the Network architecture.   

2. **Improved Efficiency**  Supporting decentralised identity at large volumes, especially with a token addition is not feasible for the current decentralised identity public utilities, which cannot handle high transaction volumes after a certain point without a substantial impact on performance.   cheqd, through Cosmos, does not hit these same bottleneck issues. For this reason, regardless of whether the token is integral to a business model or not, the Network is simply a more performant version of what is out there currently.  
3. **Cosmos champions interop**  As already mentioned, Cosmos has solved the issue of interop for tokens cross-ledger. Even if other ledgers solve the Network-of-Network problem for DIDs, they would still face token interop problems going forward.   cheqd presents itself as a sensible place to root identity primatives because its roadmap provides the most broad potential value.  
4. **Token Optionality**  Tokens for Verifiable Credential use cases may not be every company's cup of tea. Most SSI vendors already have sound business models and we understand that.   Yet, we do believe that tokens for Verifiable Credentials will begin to catalyse further real world use of SSI. And we want the industry to be able to benefit from this if they want to, without having to build it themselves.  What's more, is regardless of whether a token use case is in your current line of thinking, you will be remunerated for running a Node with block rewards and transaction fees. 

## Credential type uncertainty 

This gives everyone in the SSI community headaches: we know.

> Person 1: Indy ZKP-CL is the most privacy preserving, let's use that
>
> Person 2: Indy ZKP-CL is not standards compliant and limits interoperability - SCREW THAT
>
> Person 3: JSON-LD & BSS+ sounds cool, solves most of the privacy issues and does cool linked data thingy's - yeah can we agree?
>
> Person 4: \*SCREAMS\* AHHHH JSON is better than JSON-LD. JSON-LD is not secure GRRRRRRRRRRRRRRRR
>
> Person 5: _tentatively_ JSON with BBS+ ? 
>
> Person 6: CBOR-LD? KERI could do cool stuff!?

Yep this is not yet sorted. And we cannot sort it by ourselves. All we can do is listen and contribute to the community and work towards unification. 

Currently, JSON-LD & BBS+ signatures seems to be the most sensible route forward for interop, especially in the short term. In the long term, we may see some new innovations which address the inherent problems with JSON-LD, but we're not there yet.

At cheqd, we have, on our roadmap, support for JSON-LD with BBS+ because we see community convergence around this. 



## Listening to the Aries sceptics 

We know you don't like Aries. We are listening, and please don't run away, give this a read first, yeah? Cheers. 

The commercialisation of SSI around Hyperledger projects has been contested by large contingents of the SSI community incessantly. 

And this is understandable. For such a new and emerging technology, collaboration and community should be paramount. There is enough slices of the SSI pie for us all to have a bite. 

Hyperledger Indy fragmented the SSI community into factions, and Aries has been tagged with the same sour taste.

Aries RFCs are not the end state for credential exchange. We need a unified 'Killer Whale Jello Salad' \(if you know, you know\).

Aries Interoperability Profile V2 is a step in the right direction, but again, only a stepping stone towards something truly interoperable. 

We believe DIF's WACI PEx is genuinely a good middleground for the community to converge around right now. And we have seen concessions made in the community, through initiatives such as the Good Health Pass around WACI.

### Is cheqd WACI yet?

In short, no not yet. We are launching initially on Aries because we are prioritising speed to market. Although everything we have said above still stands true.

So, what are we doing to become collaborative and more interop focussed going forward?

We are getting our core team involved in [DIF](https://identity.foundation/), specifically

* [Claims & Credentials](https://identity.foundation/working-groups/claims-credentials.html)
* [WACI work](https://github.com/decentralized-identity/waci-presentation-exchange)
* [DIF interop](https://identity.foundation/interop/)
* [DIF applied crypto](https://identity.foundation/working-groups/crypto.html)

We are also going to work in:

* [ToIP Utility Foundry WG](https://wiki.trustoverip.org/display/HOME/Utility+Foundry+Working+Group)
* [ToIP Governance WG](https://wiki.trustoverip.org/display/HOME/Governance+Stack+Working+Group)

As said before, we want to help unite the community. 

Utilising cheqd, and joining as a Node Operator should not be seen as picking a political allegiance in the community, it should be seen as a sensible decision for decentralisation, efficiency, interop, future token use cases and remuneration for operating a Node. 



