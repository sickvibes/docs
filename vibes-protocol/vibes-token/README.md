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

{% page-ref page="treasury-allocations.md" %}

{% hint style="warning" %}
**Currently the treasury is managed by an EOA secured by a hardware wallet.** Once Gnosis ships their Safe product on Polygon \(see [this article](https://blog.gnosis.pm/gnosis-safes-multichain-future-b676b5b8f431)\), managed funds will be transferred to a safe controlled by the VIBES multisig, and the minter role on the token contract will be permanently removed.

In addition, on-chain mechanisms to lock and vest funds over time may be deployed for further decentralization and safety.
{% endhint %}

