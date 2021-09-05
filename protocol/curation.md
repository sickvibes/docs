# 🔥 Curation

Curators decide what art belongs in the VIBES collective. They have the ability to _infuse_ any NFTs they own with **VIBES**, curating them into the network.

Infusion is a process that stakes **VIBES** inside of an NFT that can be mined and claimed over time by whoever owns it. This creates a circular token economy, where **VIBES** from curated art are mined by collectors that then get to shape the future direction of the curated network.

{% page-ref page="mining-vibes/" %}

{% hint style="info" %}
Curators are onboarded via a decentralized peer-to-peer process, ensuring that no central gatekeepers are responsible for deciding the curatorial direction ****of the collective.
{% endhint %}

## Infusion

Infusion is the low-level mechanism that enables curation. Only VIBES Curators with **Influence** can infuse NFTs. What NFTs a curator infuses \(and how much they infuse\) is entirely up to them, but there are a few on-chain constraints:

**An NFT can only be infused once**. After an NFT has been curated into VIBES, it is always a VIBES NFT, even if all of the **VIBES** inside of it have been mined and claimed. There is no way to "refill" an NFT once it has fully mined all **VIBES**.

**There are limits around daily rate and total amount infused**. These parameters can be adjusted by the [VIBES multisig](governance.md#vibes-multisig) if the community finds it necessary. Currently, the mining rate is locked to 1,000 **VIBES** / day, and total infused **VIBES** must be between 50,000 and 1,095,000 \(50 days - 3 years\).

**An NFT must be owned by the person infusing it.** This can be disabled in the future by the [VIBES multisig](governance.md#vibes-multisig) if needed. The intent is that the curator must have "control" of the NFT and intersect with its on-chain provenance in order to have the ability to curate it.

{% hint style="info" %}
View the on-chain parameters around infusion constraints on the [Protocol Info](https://www.sickvibes.xyz/protocol) page under the Infusion Pool section.
{% endhint %}

## Influence

An address can have a certain amount of **Influence**, which is an on-chain value \(but not a token\). You can view your Influence on the [Wallet Page](https://sickvibes.xyz/wallet) on the VIBES site.

**Any address that has more than zero Influence is considered a VIBES Curator.**

Whenever a curator infuses an NFT to curate it into VIBES, their Influence is reduced by the same amount. This happens regardless of whether the VIBES come from their wallet or the curation grant pool.

In addition, a curator may transfer some or all of their Influence to another address, onboarding another curator. This decentralized and peer-to-peer onboarding approach ensures the VIBES network will foster a rich diversity of thought, taste, art, and voice.

{% hint style="info" %}
You can see all addresses that have been assigned Influence on [Curators List](https://sickvibes.xyz/curate/curators) page.
{% endhint %}

