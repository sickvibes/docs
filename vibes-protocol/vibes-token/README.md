# ✌️VIBES Token

**VIBES** is a [governance](../../community/governance.md), utility, and coordination tool for the VIBES cryptonetwork. **VIBES** holders own a portion of the network equity of VIBES, allowing them to influence the direction of the protocol and art collective through various governance mechanisms.

**VIBES** is not a currency nor representation of financial value. It is not a reserve-backed token. It is an experimental digital asset that explores the consequences of tokenizing the act of holding art over time in a process called [Provenance Mining](../provenance-mining.md).

{% hint style="danger" %}
Like all tech, products, and programs in VIBES, this token is an experiment. Proceed at your own risk.
{% endhint %}

{% page-ref page="where-to-get-vibes.md" %}

{% page-ref page="how-to-use-vibes.md" %}

## Token Specification

**VIBES** is a standard ERC-20 token, which is a fungible token standard compatible with nearly every Ethereum/Polygon software and hardware wallet. The token parameters are as follows:

* **Token address**: `0xd269af9008C674B3814b4830771453D6a30616eb` \([polygonscan](https://polygonscan.com/token/0xd269af9008c674b3814b4830771453d6a30616eb)\)
* **ERC-20 name:** VIBES
* **ERC-20 symbol**: VIBES
* **ERC-20 decimals**: 18

The token has no pausing functionality but there is an active minter role being held by the Treasury EOA for the time being. This may be revoked once a Gnosis Safe can be deployed for the VIBES multisig on Polygon sometime in July 2021.

Token holders may burn their tokens, which transfers to the zero-address and decreases the `totalSupply` reported by the token contract.

The token contract is verified on [polygonscan](https://polygonscan.com/token/0xd269af9008c674b3814b4830771453d6a30616eb).

{% hint style="info" %}
See [Architecture](../../resources/architecture.md) for all contract addresses and more information.
{% endhint %}

## Supply and Current Allocations

The initially minted supply for **VIBES** was 1,000,000,000 \(1 billion\) to the Treasury EOA.

Currently, funds have been allocated and distributed incrementally:

* **1,350,000 VIBES** Airdrops
* **3,000,000 VIBES** Community Programs
* **60,000,000 VIBES** Provence Mining Grant Programs

Unallocated funds are held by the Treasury EOA.

There is no target total supply or total allocation percentages at this time, and **funds will continue to be allocated incrementally while the protocol is in early development**.

{% hint style="warning" %}
**Currently the treasury is managed by an EOA secured by a hardware wallet.** Once Gnosis ships their Safe product on Polygon \(see [this article](https://blog.gnosis.pm/gnosis-safes-multichain-future-b676b5b8f431)\), managed funds will be transferred to a safe controlled by the VIBES multisig, and the minter role on the token contract will be permanently removed.

In addition, on-chain mechanisms to lock and vest funds over time may be deployed for further decentralization and safety.
{% endhint %}

## Founders Airdrop Program

An initial **VIBES** airdrop program ran roughly until July 12th 2021, which included the following recipients:

* Top 20 collectors on Screensaver v0 and v1 contracts
* All holders of **BVAL** or @bvalosek NFTs on Ethereum
* All collectors of @bvalosek Screensaver art
* All artists collected on Screensaver by @bvalosek
* Anybody showing genuine interest in the project during this time

The following amounts where airdropped:

* **10,000 VIBES** to all addresses on the airdrop list
* **10,000 VIBES** to the nine addresses that voted on the initial test proposal
* **10,000 VIBES** to anybody providing at least 5,000 VIBES worth of VIBES-MATIC liquidity on QuickSwap

The goal of this airdrop was to distribute network equity to small artists, collectors, and crypto enthusiasts in the space and encourage a grassroots bootstrapping of market liquidity. Using large DeFi airdrop lists, targeting influencers and famous artists, or launching the protocol with liquidity mining on day 1 were all intentionally avoided to ensure opportunistic whales did not end up with large amounts of **VIBES**.

All recipients of the initial airdrop are considered **Founding Members** of VIBES.

{% hint style="info" %}
Roughly **1,350,000 VIBES** where distributed during this airdrop.
{% endhint %}

## Provenance Mining Grant Program

The primary distribution method of VIBES is [Provenance Mining](../provenance-mining.md), which is managed autonomously by locking VIBES from the treasury into the [VIBES Wellspring contract](../../resources/architecture.md). 

The Provenance Mining Grant Program allocates funds from the **VIBES** treasury to be seeded into NFTs created by VIBES artists. 

This is currently a permissioned process gated by the VIBES multisig.

| Program | Date | Amount | Info |
| :--- | :--- | :--- | :--- |
| v1 | June - July 2021 | 30,000,000 **VIBES** | Initial launch with @bvalosek's art |
| v1.1 | July - August 2021 | 30,000,000 **VIBES** | Initial multi-artist launch \([proposal](https://snapshot.org/#/sickvibes.eth/proposal/QmdwL7CMqaDjha3nJvm69HtHjUSH5Ma8ozhxm7YF4aYiRh)\) |

## Community Programs

Community Programs are used to fund builder stipends and community bounties, which are used to compensate contributors to the VIBES protocol. 

All community program funds are distributed via the VIBES multisig.

| Program | Date | Amount | Info |
| :--- | :--- | :--- | :--- |
| v1 | July 2021 | 3,000,000 **VIBES** | Initial community program \([proposal](https://snapshot.org/#/sickvibes.eth/proposal/QmdwL7CMqaDjha3nJvm69HtHjUSH5Ma8ozhxm7YF4aYiRh)\) |

