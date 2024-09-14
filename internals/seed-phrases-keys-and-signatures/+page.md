---
title: Seed phrases, keys & signatures
description: 'Understand how seed phrases, private keys, public keys, and signatures ensure the security and integrity of your cryptocurrency wallet.'
---

<script>
	import {KeyTakeaways} from "$modules/knowledge-base"
</script>

Cryptocurrency wallets are essential tools for managing and securing digital assets, enabling users to store and transfer cryptocurrencies or other tokens and to interact with blockchain. At the core of these wallets are seed phrases, private keys, public keys and signatures - four fundamental components that take part in ensuring the authenticity and integrity of the blockchain.

#### Seed phrase

When a new cryptocurrency wallet is created, the wallet software generates a seed phrase. Most commonly, seed phrases consist of 12, 18 or 24 **human-readable words** designed to be easy to understand, store, and remember. Their simplicity and memorability makes them an effective **backup mechanism** for securing and recovering your wallets.

The seed phrase plays a crucial role, as it is used to derive a **master seed**. The master seed, in turn, is used to **generate private keys**. This is why your wallet provides you with a single seed phrase but allows you to create multiple addresses, each with its own private key. This hierarchical structure makes managing multiple accounts both secure and convenient.

#### Private key

A private key is a **long alphanumeric string** generated through complex encryption algorithms. It grants **full access** to the associated wallet, so it is crucial to keep both the private key and the originating seed phrase secure and **never share** them with anyone.

To validate wallet ownership, the private key is used to generate public keys and signatures, which can be freely shared publicly.

#### Public key

A public key is derived from the private key and **allows others to verify** that a message or transaction was signed by the holder of the respective private key without revealing the private key itself. A **wallet address** is a short and user-friendly representation of a public key.

This mechanism is not exclusive to blockchain and cryptocurrencies but is also the standard for secure and private communication over the internet. The feature is enabled through **asymmetric cryptography**. The relation between the private and public keys is based on mathematical principles that make it easy to **generate a public key from a private key**, but not the other way around.

To illustrate such **one-way functionality** with a simplified example, consider the modulo operation. Representing the private key with a large number, we can easily compute its modulo value. However, given the result, it is infeasible to perform a reverse operation to determine the original value of the private key.

#### Signature

A signature is also derived from the private key. When a transaction or message is created, the data is hashed and then encrypted with the private key, resulting in a digital signature. This signature is attached to each on-chain interaction and can be viewed through a blockchain explorer.

To verify the authenticity of the signature, anyone can use the **public key to decrypt the signature** and compare the decrypted hash with the hash of the original data. If they match, it **confirms the data’s authenticity** and integrity.

<KeyTakeaways items={[
"<b>Seed phrase:</b> A seed phrase is a vital backup tool consisting of words that generate your wallet’s private keys and enable secure recovery of your wallet.",
"<b>Private key:</b> A private key is an alphanumeric string that provides complete access to your crypto wallet, making it essential to keep it confidential and protected.",
"<b>Public key & signature:</B> Public keys and signatures are used to verify transactions and messages on the blockchain, ensuring authenticity without revealing your private key."
]} />
