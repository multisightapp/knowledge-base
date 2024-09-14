---
title: Action execution
description: 'Discover how multisignature wallets handle action execution, including finalizing decisions, managing network gas fees, and the impact of action order.'
---

<script>
	import {KeyTakeaways} from "$modules/knowledge-base"
</script>

Execution is the final step in processing an action within a multisignature wallet. It carries out the collective decision to transfer assets, initiate a smart contract interaction, or update the multisig configuration.

Once an action has been **confirmed** by the required number of owners, it becomes **eligible for execution**. Depending on the wallet’s implementation and configuration, execution may occur automatically or require manual initiation by an owner. At this stage, the action is removed from the pending queue and pushed to be processed on the blockchain.

Gas fees are one of the key considerations during this stage, as they cover the costs of processing the action on the blockchain. High gas fees can affect both the speed and cost of execution, making it essential for wallet owners to manage these costs effectively. Understanding potential **fluctuations in gas prices** and planning accordingly can help ensure that actions are **executed efficiently**, avoiding unnecessary delays or expenses - similar to regular crypto wallets.

In many multisig wallets, the user who triggers execution pays the gas fees from their account. However, some wallets allow these fees to be paid directly from the multisig’s own funds. This feature simplifies the process by ensuring that the wallet itself covers the costs, making execution smoother and less dependent on individual owners’ ability to pay upfront and manage reimbursements later.

The order in which actions are executed also varies among multisignature wallets. Some wallets require actions to be executed **in the order** they were submitted, particularly when actions are interdependent. This helps prevent errors and ensures that transactions are carried out correctly. Other wallets allow actions to be executed **out of order**, providing flexibility to prioritize certain actions based on urgency or strategic needs. Owners of wallets that require ordered execution must be mindful of the action sequence, as delays in confirming earlier actions can hold up subsequent ones. Conversely, wallets that permit unordered execution offer more flexibility but require careful management to avoid potential issues.

<KeyTakeaways items={[
"<b>Finalizing the action:</b> Execution is the final step in a multisig wallet, where confirmed actions are carried out, including transferring assets, interacting with smart contracts, or updating configurations based on collective decisions.",
"<b>Costs & delays:</b> During execution, gas fees are a crucial consideration, impacting both the speed and cost of processing on the blockchain. Effective management of these fees is essential to ensure actions are completed efficiently and without unnecessary expenses.",
"<b>Order vs. flexibility:</b> Multisigs vary in how they handle execution order. Some process actions sequentially to maintain accuracy, while others offer flexibility to prioritize actions based on urgency or strategic needs."
]} />
