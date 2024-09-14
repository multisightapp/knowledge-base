---
title: Introduction to multisignature wallets
description: 'Learn how multisig wallets improve crypto security by distributing control, requiring multiple approvals for transactions, and offering flexible setups.'
---

<script>
	import {KeyTakeaways, ARTICLES} from "$modules/knowledge-base"

	const LINK_KEYS_AND_SIGNATURES = ARTICLES['seed-phrases-keys-and-signatures'].href
</script>

Multisignature wallets, or **multisig** wallets, are a powerful way to **enhance security and distribute control** when managing **crypto assets**. Unlike regular wallets that rely on a single person and a single private key, multisig wallets require **multiple approvals to authorize actions**.

#### Enhanced security

One of the main advantages of multisig wallets is the added security they provide. In a traditional wallet, a single <a href={LINK_KEYS_AND_SIGNATURES}>private key</a> grants full access to the stored funds and controlled smart contracts. If the key is lost, stolen, or compromised, the assets are at risk. In contrast, multisig reduces this vulnerability by **requiring multiple keys** to authorize any action.

For instance, a 2-of-3 multisig wallet requires two out of three available key owners to sign off on any action. Even if **one key is compromised**, the attacker still **cannot control the wallet** without the others. This significantly reduces the likelihood of theft or unauthorized access, making multisignature wallets ideal for both personal savings and shared high-value holdings.

Based on the same principle, multisig wallets also provide a more secure **backup solution**. Instead of relying on a single key, users can store **multiple keys across different devices or locations**, ensuring that losing one key doesn’t result in the total loss of access and funds. This layered security approach helps both individuals and groups better protect their assets.

#### Distributed control

Another key feature of multisig wallets is the ability to **distribute control among multiple people or devices**. In a traditional wallet, only one person holds the key, meaning they have sole control over it. While this may be convenient for personal use, it can pose risks in group settings where consensus is important.

With a multisignature wallet, **ownership is shared among multiple parties**. Whether it’s family members, business partners, or a group of community members, multisig allows everyone to take part in the decision-making process. This is especially powerful in groups where **decisions need to be made together** to ensure trust and accountability.

#### Flexible configuration

A compelling benefit of multisig wallets is also their customizability. Users can choose and configure a setup that fits their specific needs:

- **Individuals:** For personal assets, you can hold multiple keys spread across different devices to enhance both security and backup options.
- **Small groups:** For assets shared among multiple people, each can hold a key, ensuring that everyone is involved in decisions about shared funds.
- **Large communities:** For community projects or decentralized organizations, ownership can be spread across many members, promoting transparency, collective management, and reducing the risk of power abuse.

<KeyTakeaways items={[
"<b>Boosting security:</b> Multisignature wallets provide added security by requiring multiple approvals to authorize actions, significantly reducing the risk of unauthorized access or theft.",
"<b>Collective decision-making:</b> By involving multiple parties in the approval process, multisig wallets promote cooperation in managing assets and require consensus before taking action.",
"<b>Customizable setup:</b>Multisig wallets offer various setup options, accommodating the specific needs of individual users, small groups, or large communities."
]} />
