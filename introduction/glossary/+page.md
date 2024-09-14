---
title: Glossary
description: 'Discover key terms in crypto and multisignature wallets, including keys, owners, signers, actions, transactions, and confirmation thresholds.'
---

<script>
	import {ARTICLES} from "$modules/knowledge-base"

	const LINK_KEYS_AND_SIGNATURES = ARTICLES['seed-phrases-keys-and-signatures'].href
	const LINK_OWNER_COUNT = ARTICLES['owner-count-and-threshold'].href
</script>

#### Crypto wallet

A **crypto(currency) wallet** is a tool that enables users to securely **store, receive, and send various types of cryptocurrencies** and tokens. It serves as an interface for interaction with the blockchain, managing the <a href={LINK_KEYS_AND_SIGNATURES}>private and public keys</a> necessary for access and control of digital assets.

Crypto wallets can be used solely as a **software** or through dedicated **hardware devices**. Each wallet, whether regular or multisignature, is represented by an address, a unique alphanumeric identifier derived from its public key.

#### Multisig

Multisig is short for **multisignature wallet**, a type of cryptocurrency wallet that typically requires **two or more private keys to authorize transactions** or perform certain actions, as opposed to a single key in a personal wallet.

#### Owner

Ownership of a multisignature wallet is **distributed among the individuals associated with the multisig**. Each individual is referred to as an owner, as they control a portion of the multisig wallet's private keys, which are linked to the addresses of their personal wallets.

#### Signers & confirmations

A signer is a term used for a multisig **owner who approves a pending action** by signing it through their crypto wallet. For an action to be executed, it must reach a predefined **<a href={LINK_OWNER_COUNT}>threshold of confirmations</a>** from the pool of owners. Therefore, the term refers to the specific combination of a multisig action and the owner involved, rather than the multisig wallet in general.

#### Actions & transactions

Actions refer to any multisig operation that requires the predefined number of confirmations. These include **basic asset transfers** and **interactions with smart contracts**, but also **functions within the multisig wallet itself**, such as updates to the owners' pool or changes to the confirmation threshold.
