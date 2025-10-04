Swapr: A Decentralized Token Swap Smart Contract on Stacks

Overview
**Swapr** is a **Clarity-based decentralized exchange (DEX)** smart contract that enables **peer-to-peer token swaps** directly on the **Stacks blockchain** without intermediaries.

This contract allows users to:
- **List** their tokens for swapping with custom price ratios.  
- **Execute** secure and trustless swaps between fungible tokens (SIP-010 compliant).  
- **Cancel** unfulfilled swaps safely.  
- **Verify** swap authenticity and balances on-chain through Clarity’s predictable, auditable logic.

---

Key Features
- **Trustless swaps:** Users retain full control until execution.
- **SIP-010 compliant:** Works seamlessly with standard Stacks fungible tokens.
- **Transparent logic:** Every transaction is verifiable on-chain.
- **Modular design:** Can be extended for liquidity pools or automated pricing (AMM).

---

Smart Contract Functionality
| Function | Description |
|-----------|--------------|
| `create-swap` | Registers a new swap offer specifying token type, amount, and desired token. |
| `execute-swap` | Completes the token exchange between the two parties if conditions are met. |
| `cancel-swap` | Allows the creator to cancel a pending swap if not yet executed. |
| `get-swap-details` | Returns stored information about a swap offer. |

---

Project Structure
-swapr
-contracts
-swapr.clar
-tests
-swapr_test.ts
-Clarinet.toml
-README.md
-LICENSE
