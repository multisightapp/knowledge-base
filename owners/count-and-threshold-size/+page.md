---
title: Owner count & threshold size
description: 'Explore how owner count and threshold size affect multisig wallet security and efficiency. Learn how to find the ideal setup for your specific use case.'
---

<script>
	import {KeyTakeaways} from "$modules/knowledge-base"
</script>

The ownership of a multisignature wallet is distributed among multiple addresses associated with the wallet. Each address is known as an owner, and each **owner controls a portion of the multisig**. To execute a pending transaction or action, a specified number of owners must confirm it with their signatures.

The combination of these two parameters is commonly specified as **M/N** or **m-of-n**, where M defines the **required number of confirmations** (the threshold), and N represents the **total number of owners** of the multisignature wallet. The threshold can range from 1 to the total number of owners - for example, configurations such as 1/3, 3/5, and 6/6 are all valid.

Every use case for multisig wallets is unique, and therefore, there is no universally recommended value for these parameters. Several factors influence the configuration: value of managed assets and controlled contracts, size of the group or community, desired level of decentralization, frequency and urgency of action executions, and more.

The vast majority of multisig wallets focus on one of two main objectives:

- **Enabling backup:** Utilizing multiple owners to prevent losing access to an important wallet.
- **Boosting security:** Utilizing multiple owners to prevent unauthorized control over shared assets.

Setting up a multisig as a backup solution emphasizes the total number of owners. By adding **more personal wallets** as owners to the multisig wallet, users **can still access the multisig** through other wallets if they lose access to one. However, this can also increase the risk of a hostile takeover - for instance, in a 1/X multisig, taking over a single wallet still grants control over the entire multisig.

To counter the risk of a hostile takeover, multisignature wallets can be configured with security as the main objective. In this setup, a higher threshold is required, meaning **multiple owner confirmations** are needed for any transaction or action. This approach is useful for individuals seeking to **protect** their important wallets **from a single point of failure** and for groups or communities **managing shared funds** or contracts, requiring broad consensus. On the other hand, this can reduce operational efficiency, as it may take longer to reach the required threshold for action.

Since most multisig solutions enable the configuration to be updated over time, you can take inspiration from publicly available setups and experiment to find the configuration that fits your use case best.

<KeyTakeaways items={[
"<b>Owner confirmations:</b> Multisig wallets require a specified number of confirmations from the total pool of owners to execute transactions or actions.",
"<b>Configurational variability:</b> There is no universal template for multisig configurations. Factors such as asset value, community size, desired level of decentralization, and action frequency influence the configuration.",
"<b>Security through majority:</b> Configurations with higher thresholds enhance security by making malicious takeovers challenging, as they rely on a majority or significant consensus for execution."
]} />
