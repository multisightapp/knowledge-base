---
title: Signature storage
description: 'Get insights into on-chain vs off-chain signature storage for multisig wallets and learn how these methods impact transaction costs, efficiency, and privacy.'
---

<script>
	import {KeyTakeaways} from "$modules/knowledge-base"
</script>

Signatures are a key component of blockchain technology, ensuring the validity and integrity of every transaction. The method of storing these signatures, whether on-chain or off-chain, has significant implications on performance, costs, and privacy. By understanding the strengths and limitations of both, you can make informed decisions on which multisignature solution to choose to optimize for your use case.

#### On-chain signature storage

On-chain storage is based on recording every **signature directly on the blockchain**. The **accessibility and verifiability** of all transaction data enhances transparency, trust, and accountability within the system, benefiting decentralized and immutable networks the most. Additionally, the process of on-chain storage is relatively straightforward, requiring no extra infrastructure beyond the blockchain itself.

However, storing each signature on-chain can significantly increase the costs of owning a multisig wallet. Each signing owner has to **pay network fees** for publishing their signature, which can accumulate quickly, especially in systems requiring multiple signatures for a single transaction, like multisignature wallets. Privacy can also be another concern, as all transaction details are publicly exposed, which may be undesirable for users prioritizing confidentiality.

#### Off-chain signature storage

Off-chain signature storage involves collecting and managing **signatures outside of the blockchain** through a separate service. Once all required signatures are gathered, they are included in the final transaction execution on the blockchain. Compared to on-chain storage, efficiency is a major advantage, as it reduces the data load on the blockchain, allowing for **faster and cheaper** signature collection. Depending on the chosen solution, privacy can also be another key benefit of this approach. By keeping interim transaction data off the public ledger until the final transaction is executed, off-chain storage can increase user privacy.

To achieve these benefits, a **custom infrastructure** next to the blockchain is required to **collect and manage signatures**. This complexity introduces **potential trust and reliability concerns**, as users depend on external services. While these services can be secure, they may still be susceptible to attacks or failures, unlike the inherent protection offered by on-chain systems.

One of the most popular multisig solutions, Safe, leverages this method by offering a custom smart contract and providing a public transaction service for the collection and management of signatures, making it convenient for the majority of users. Moreover, their code is **audited and open-sourced**, enabling more advanced users to deploy and manage their **private transaction service**.

<KeyTakeaways items={[
"<b>On-chain storage:</b> Recording signatures on-chain enhances transparency and trust in decentralized systems but incurs higher costs and compromises privacy due to the public availability of transaction data.",
"<b>Off-chain storage:</b> Off-chain storage offers a more efficient and private solution by handling signatures externally, though it depends on external services that might pose trust and security challenges."
]} />
