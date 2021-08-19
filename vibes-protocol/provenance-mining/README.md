# 💎 Provenance Mining

Provenance Mining is a core VIBES protocol feature that allows **VIBES** tokens to be mined over time inside of an NFT.

The mined **VIBES** stay within the NFT across sales or transfers, and claiming VIBES is a one-way operation that only the owner of the NFT can perform.

{% hint style="info" %}
This is the foundational experiment of VIBES: **What happens when tokenize the act of holding art over time?**
{% endhint %}

## What?

Provenance mining is a crypto experiment_._ It gives artists the primary role of capital distribution in a crypto network and allows collectors to capitalize on their support of an artist over time.

This could go a lot of ways, **which is exactly why we're building it**. 

Aren't you curious to see how this plays out? ****🤔

{% hint style="info" %}
If you want to dive deep on the ideas around provenance mining, [check out the Protocol Thesis writeup](protocol-thesis.md) that covers several potential outcomes and use cases of this concept.
{% endhint %}

## Infusing NFTs with VIBES

An artist can infuse any NFT they own with **VIBES,** either from their wallet or via [Provence Mining Grants](../vibes-token/treasury-allocations.md#provenance-mining-grant-program). 

Each VIBES NFT has its own supply of **VIBES** and each NFT is fully independent. Infused **VIBES** cannot be accessed or removed by anyone except through provenance mining them over time, and the mining rate cannot be changed or stopped once started.

{% hint style="info" %}
This is currently a permissioned process that only the VIBES multisig can perform and is [limited to hand-selected artists](../../community/artists/#provenance-mining-grant-recipients). 
{% endhint %}

## Claiming Mined Tokens

Mined tokens can be claimed by the owner of the NFT at anytime \(as long as it isn't locked\), but tokens cannot be put back in the NFT after the initial supply has been infused.

The NFT owner can use the [VIBES UI](https://sickvibes.xyz) to claim tokens, or chose to directly interact with the [VIBES Wellspring contract](../../resources/architecture.md#smart-contract-architecture) in the case that the site is no longer available.

Claiming tokens does not stop the mining process and new tokens will continue to be mined so long as there are **VIBES** remaining from the initial infused supply. Mined tokens can be claimed indefinitely, even after the entire supply has been mined.

Unclaimed tokens stay within the NFT across sales or transfers, and mining continues until supply runs out regardless of the current owner.

## Locking Tokens

A token can be locked by the token owner at any time. Locking a token **does not prevent sales or transfers**, but it does prevent claiming any of the mined **VIBES**. 

A token will automatically unlock after 30 days, or the owner may trigger a time-delayed unlock that will unlock the token after a 24 hour cool down.

The NFT owner can use the [VIBES UI](https://sickvibes.xyz) to lock tokens, or chose to directly interact with the [VIBES Wellspring contract](../../resources/architecture.md#smart-contract-architecture) in the case that the site is no longer available.

The locking mechanism exists to prevent a front-running attack where a seller could claim the **VIBES** in an NFT right before the sale or transfer, resulting in the buyer holding an NFT that had be "drained" at the last moment.



