---
title: Action confirmation
description: 'Explore action confirmation in multisignature wallets, focusing on how careful verification of transaction details ensures security and prevents errors.'
---

<script>
	import {KeyTakeaways} from "$modules/knowledge-base"
</script>

Action confirmation is a critical and defining feature of multisignature wallets. It is the process where the **security and integrity of the wallet** are upheld or compomised. Every action confirmation demands meticulous **attention and informed decision-making** by all involved participants.

After an action is submitted within a multisig wallet, it enters a queue of pending actions **awaiting review and confirmation**. For the action to become executable, it must receive a **predefined number of confirmations** from the wallet's owners. Each involved owner must carefully verify the accuracy and origin of all action details, including:

- **Involved addresses:** Ensure that the recipient addresses are correct and belong to the intended parties.
- **Token types:** Verify that the correct tokens or cryptocurrencies are being transferred or interacted with.
- **Amount of assets:** Confirm that the ammount of assets involved is correct.
- **Function calls:** Review any calls, parameters or arguments in the transaction, such as data for smart contract interactions.

It's also crucial to cross-check these details against the original action proposal. A discrepancy as small as a single character in an address or amount can result in the **permanent loss of funds or control over critical contracts**. Proactive communication among wallet owners and other involved parties is encouraged, and open discussion about potential issues or misunderstandings should be part of the review process.

Many multisig wallet interfaces provide features to aid in the confirmation process, making the details more accessible and easier to understand. These can include labeling of known addresses, alerts for unfamiliar tokens, state change summaries, action simulation, and more.

While it is desirable for multisig owners to respond to incoming actions within a reasonable timeframe, security should never be compromised for speed. Each owner should permorm their **due diligence** and resist internal or external pressure to act swiftly. Threats like hostile account takeovers or social engineering attacks can occur, so owners should balance the need for timely execution with the **thorough and accurate review**.

If an error or malicious modification is detected during the confirmation stage, or if the circumstances of the action change, it may need to be canceled. Depending on the wallet's configuration, canceling might require approval from a predefined number of owners or other designated users. After cancelation, the action can be resubmitted with the correct details, re-initianting the entire process.

Some multisig smart contracts also support action confirmations by community members through voting power of their governance token holdings or other conditions. When setting up a multisignature wallet, all risks accompanied with this approach should be carefully considered.

<KeyTakeaways items={[
"<b>Security through concensus:</b> Confirming actions in multisig wallets is crucial for maintaining security. Actions must receive a predefined number of confirmations from owners to ensure agreement and integrity.",
"<b>Accuracy over speed:</b> While quick responses are desirable, multisig owners must focus on accurate and thorough reviews. Avoiding hasty decisions is essential to prevent errors and maintain security."
]} />
