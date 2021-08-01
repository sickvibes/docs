# 🏛️ Governance

VIBES is a decentralized [cryptonetwork](../vibes-protocol/vibes-token/) that is owned by the community. If you hold **VIBES**, own NFTs with **VIBES** staked inside of them, or are supplying market liquidity for **VIBES** - you have _vote power_ in the protocol. 

{% hint style="info" %}
Using your vote power to influence, control, or direct the protocol via off-chain signaling or on-chain voting is known as **digital governance**.
{% endhint %}

## Vote Power

Your VIBES vote power is a reflection of your portion of the equity you have in the VIBES cryptonetwork. 

The more vote power you have, the more influence and control you have over the protocol.

{% hint style="info" %}
Go to [sickvibes.xyz/wallet](https://sickvibes.xyz/wallet) to see your vote power.
{% endhint %}

### Membership Threshold

Currently, you must have **10,000 vote power** to get the [VIBES Member Discord role](../resources/guides/how-to-get-vibes-discord-roles.md) required to chat in the Governance channel or create a new Snapshot proposal.

{% page-ref page="../vibes-protocol/vibes-token/where-to-get-vibes.md" %}

There are no requirements to be a contributor or chat in the main Discord channels.

### Details

Vote power calculation for VIBES happens entirely on-chain via the [Vote Power Adapter](../resources/architecture.md) smart contract. The strategies used can be dynamically set by the VIBES [multisig](governance.md#vibes-multisig).

Currently, vote power is the sum of the values calculated from the following strategies:

* Current **VIBES** held in your wallet
* Underlying supply of **VIBES** for **VIBES-MATIC LP** held in your wallet. This can change over time as the market price of **VIBES** on the exchange changes. 
* Claimable **VIBES** within any VIBES NFTs currently held in your wallet. This will change over time as more **VIBES** are mined or **VIBES** are claimed. If you sell or transfer the NFT without [claiming](../resources/guides/how-to-claim-vibes-from-an-nft.md) the mined **VIBES**, your vote power will drop.

{% hint style="info" %}
The upcoming [Governance Farming](../vibes-protocol/governance-farming.md) program will inflate the vote power contribution from being an LP.
{% endhint %}

## Process

VIBES is a process-minimal organization, but below is a rough outline of how we coordinate governance.

### Discord Discussion

Protocol governance starts with informal discussion on Discord. Have an idea? Want to see something changed? Float it in the chat and see what others think. 

{% hint style="info" %}
Use the [\#🏛️**-governance** channel ](https://discord.gg/C5TFZVjSZ5)on Discord to discuss any ideas for changes or possible future proposals for VIBES.
{% endhint %}

### Off-chain Signaling

VIBES uses [Snapshot](https://snapshot.org/#/sickvibes.eth) for off-chain signaling, which lets you securely vote by using your web3 wallet to cast a signed ballot. 

{% page-ref page="../resources/guides/how-to-vote-on-snapshot.md" %}

Off-chain signaling is great for gauging community consensus around how to use shared resources or signal support for a change in the protocol. Feel free to use Snapshot in more creative ways if you think it'd be helpful or fun.

Don't feel like a Snapshot proposal needs to be created for everything \(we build first and ask for permission later\), but it can be a great way to encourage community involvement and allow people to voice their opinion

{% hint style="info" %}
**Snapshot is just a tool**: since it's not on-chain it's not binding except at the "social layer". 
{% endhint %}

## Organization

The organization of VIBES is intentionally very flat, simple, and non-prescriptive.

We are an early-phase protocol and are avoiding having explicit roles and favor open, permissionless contribution. 

{% page-ref page="contributing.md" %}

### VIBES Multisig

The VIBES multisig members where chosen by @bvalosek in the initial phases of VIBES based on mutual trust, friendship, crypto fluency, and support of both the VIBES project and the [BVAL NFT project](../resources/updates/prologue.md) that started it.

The multisig is a social-layer coordination group, and Gnosis Safe has been deployed to manage protocol assets and smart contract control. 

{% hint style="info" %}
All on-chain actions and off-chain agreements requires **3-of-5 consensus** among multisig members.
{% endhint %}

The address of the multisig Gnosis Safe:

* `0x41925458151134A5324c9382915fc94C31Bce1B3` \[[polygonscan](https://polygonscan.com/address/0x41925458151134A5324c9382915fc94C31Bce1B3)\]

The multisig is responsible for:

* Handling [VIBES Treasury](../vibes-protocol/vibes-token/treasury-allocations.md) funds
* Determining [community stipend](contributing.md) payouts
* Selecting the initial artists to receive provenance mining [grants](../vibes-protocol/vibes-token/#provenance-mining-grant-program) 
* [Smart Contract](../resources/architecture.md) administration and protocol control
* Snapshot Space configuration
* Discord administration

#### VIBES Multisig Members

Members can be identified in Discord via the **@VIBES multisig** role.

| Name | Discord | Info |
| :--- | :--- | :--- |
| Brandon | `bvalosek#9578` | \[[polygonscan](https://polygonscan.com/address/0x303eefedee1ba8e5d507a55465d946b2fea18583)\] |
|  | `zamboni#2731` | \[[polygonscan](https://polygonscan.com/address/0x8AbAf5733742B1506F6a1255de0e37aEc76b7940)\] |
|  | `leesah#3235` | \[[polygonscan](https://polygonscan.com/address/0xf8530CcA204442e56F8f55ea35Eb0fDF0b40eEc8)\] |
|  | `lootsoot#7959` | \[[polygonscan](https://polygonscan.com/address/0x0c6204B8ebaF837d5cff51447050777CD9B39FC4)\] |
|  | `jpangelle#5070` | \[[polygonscan](https://polygonscan.com/address/0xf976128e5c9214F802184A3d6f97DdEeEa78c124)\] |

{% hint style="info" %}
**Please do not DM members of the multisig** regarding any administrative questions or requests, ask in public Discord channels and tag the **@VIBES Multisig** role.
{% endhint %}

