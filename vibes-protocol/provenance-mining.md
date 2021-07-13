# 💎 Provenance Mining

Provenance Mining is an on-chain network equity distribution mechanism where claimable **VIBES** are mined over time inside of an NFT. 

The mined **VIBES** stay within the NFT across sales or transfers, and claiming VIBES is a one-way operation that only the owner of the NFT can perform.

{% hint style="info" %}
This is the foundational experiment of VIBES: **What happens when tokenize the act of holding art over time?**
{% endhint %}

## Protocol Thesis

Provenance Mining is really a test in prod, but the hope is that exploring this concept will lead to interesting conclusions and discoveries. Below are a few things that provenance mining _might_ end up being.

### Token Distribution

An artist can distribute or sell NFTs among their collectors, community, or fans. Each NFT acts a "portal" that continuously streams mined tokens that can be claimed by the NFT owner. This allows an artist to distribute network equity among people who are interested in the art or project in a very tangible way.

Injecting the NFT can only occur once, but it can occur much later than the token was minted. An artist could chose to inject the distributed token only _after_ the NFTs have been fairly distributed, "switching on" the provenance mining at a later time. 

### Instrumentation of Value

Crypto, and specifically programmable blockchains, offer equitable and democratized access to powerful coordination technology. Provenance mining may be a new way of instrumenting \(or representing / tokenizing\) the _value_ of holding an artist's work over time in way that was not possible in the past. 

Traditionally, the only way to capture value has been with _money_, which is at best a lossy abstraction of value. With the composability of crypto, we now have the ability to instrument all types of value that we couldn't before. 

Once you can effectively instrument something abstract like "the value associated with holding art over time", you can now "tether" it to other forms of values via markets and or other on-chain mechanisms. 

### Value Circulation

A collector could hold art for a while and thus mine a lot of tokens over time. The art would have intrinsic value as a piece of artwork minted by the artist, but its provenance is directly represented by the mined tokens inside of it. 

The collector could decide to claim all of the mined tokens, and then resell the art. This could allow the collector to capitalize on the value of holding art over time \(by selling the claimed tokens\), while reselling the art to another collector \(potentially for less, since all tokens are claimed\).

This could create an interested _cycle of value_ where collectors mine provenance over time, capitalize on that provenance, and then re-sell the NFT to somebody else to do the same thing.

### Collective Value Socialization

If more than one artist is minting NFTs that provenance mine the same token, the token now represents the amalgam of value associated with holding that collection of artists' art over time. This can be a way of socializing the value \(and thus potential revenue / demand\) of art across a group of artists, potentially with varying degrees of existing demand or revenue-generating potential.

An artist collective could bring on new or undiscovered artists, allowing them to mint art injected with the mineable token. This gives the art additional intrinsic value since collectors can mine the effective "composite value" of the provenance of all artists in the collective.

## Mechanics and Concepts

All provenance mining interactions are handled by the [VIBES Wellspring contract](../resources/architecture.md).

### Seeding the Initial Supply

An NFT can be seeded / injected with **VIBES** just once, there is no topping off of **VIBES**. The lifetime mineable supply of **VIBES** for a token is locked in the [VIBES Wellspring contract](../resources/architecture.md), with no way to remove the funds unless the token is burnt.

Each VIBES NFT thus has a finite supply of **VIBES.** This is the effective "total lifetime value" of the provenance mining that can occur for a given NFT. After all of the initial supply of VIBES for a NFT are mined, no more **VIBES** will be generated. Claiming the **VIBES** can happen indefinitely so long as there are some remaining, even after mining has stopped.

**VIBES** are mined from the initially staked supply in the VIBES Wellspring into "claimable" VIBES that the owner can unstake at a linear immutable rate.

### Claiming and Locking

At any time, the owner of an NFT can claim the currently minted VIBES from any NFT they own \(if the NFT is not locked\). The owner can claim some or all of the currently claimable VIBES, which is a one-way operation. 

A token can be _locked_ by the token owner at any time. Locking a token does not prevent sales or transfers, but it does prevent claiming any of the mined VIBES. A token will automatically unlock after 30 days, or the owner may trigger a time-delayed unlock that will unlock the token after 24 hours.

The locking mechanism exists to prevent a frontrunning attack where a seller could claim the VIBES in an NFT before the sale or transfer transaction is mined, resulting in the buyer holding an NFT that had be "drained" at the last second.

