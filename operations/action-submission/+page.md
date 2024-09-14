---
title: Action submission
description: 'Learn how to submit actions in multisignature wallets — propose transactions, review details, and prepare other signers for a smooth confirmation process.'
---

<script>
	import {KeyTakeaways} from "$modules/knowledge-base"
</script>

Action submission is the initial step in any transaction or operation within a multisignature wallet. It allows wallet owners to **propose actions** such as transferring assets, interacting with smart contracts, or modifying wallet configurations. This process **sets up the necessary details** for the action, which will later require confirmation from others before execution.

In both regular and multisig wallets, the process begins by specifying the action details. These typically include the **addresses involved, the amount of assets, function calls, or any other relevant data**. After entering all the required information, the submitter reviews the details within the wallet's interface. This review is crucial because once the action is submitted, it becomes immutable, preventing any tampreing or accidental changes, and safeguards the integrity of the process. Any errors discovered after this stage can only be addressed by canceling and resubmitting the action.

In multisig wallets, action submisssion does not immediately lead to execution. Instead, the **action enters a queue** of pending proposals. Each action must reach the required threshold of confirmations from other owners before becoming executable.

Not all actions typically associated with crypto wallets are feasible in multisig wallets. Actions that rely on immediate execution, such as spontaneous transactions (e.g. NFT minting) or high-frequency trading requiring real-time adjustments, are generally not practical in a multisig setup. When using a multisignature wallet, it's important to consider whether the actions align with the wallet's **need for consensus** and the potential **delays in execution**.

Some multisig smart contracts also allow action submission by any address that meets specific criteria, such as holding a set amount of a particular governance tokens or fulfilling other predefined conditions. This approach provides flexibility and inclusivity, allowing projects to involve community members beyond just multisig owners, while still maintaining security and a reasonable level of control.

<KeyTakeaways items={[
"<b>Initiating a proposal:</b> Action submission starts the transaction process in a multisig wallet by detailing involved addresses, assets, smart contract functions, and other relevant information.",
"<b>Delayed execution:</b> Multisig actions need approval from multiple owners, which introduces delays and makes them unsuitable for real-time or high-frequency transactions."
]} />
