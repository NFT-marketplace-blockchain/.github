# Nexus Protocol

A high-performance, decentralized NFT marketplace ecosystem incorporating Account Abstraction (ERC-4337) and a scalable event-driven architecture.

## Ecosystem Overview

The system is composed of four primary components working in tandem:

| Component | Repository Name | Local Path | Tech Stack | Description |
| :--- | :--- | :--- | :--- | :--- |
| **Smart Contracts** | `contracts-core` | `/blockchain` | Hardhat, Solidity | Core marketplace protocol and Account Abstraction infrastructure. |
| **API Service** | `api-service` | `/back-end` | FastAPI, Python | Off-chain indexer, REST API, and WebSocket gateway. |
| **Web Client** | `web-client` | `/frontend-nextjs` | Next.js 15, Wagmi | Primary user interface for trading and asset management. |
| **Admin Portal** | `admin-portal` | `/frontend-admin` | Vite, React | Dashboard for system operations and management. |

## Architecture

1.  **Blockchain Layer**: Smart contracts deploy on EVM-compatible networks, managing asset ownership (ERC-721/1155) and trading logic.
2.  **Indexing & API**: The backend service listens for blockchain events to maintain a high-speed off-chain database, serving complex queries that are expensive to run on-chain.
3.  **Frontend Clients**:
    *   **USER**: Connects via Web3 wallets (or email via Account Abstraction) to interact with the marketplace.
    *   **ADMIN**: Provides oversight on campaigns, users, and system configurations.

## Development Status

*   **Logic**: Feature-complete for core trading flows.
*   **Infrastructure**: Local development environment configured with Hardhat node.
*   **UI/UX**: Modern implementation using Shadcn UI and specialized Web3 hooks.

---
*Documentation for the KLTN Project.*
