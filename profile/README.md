# ArtChain-NFT

A high-performance, decentralized NFT marketplace ecosystem built with Account Abstraction (ERC-4337) and a scalable event-driven architecture.

## Architecture Overview

The ecosystem consists of four specialized services working in unison:

### Core Services

| Service | Repository | Technologies | Description |
| :--- | :--- | :--- | :--- |
| **Smart Contracts** | [contracts-core](https://github.com/NFT-marketplace-blockchain/contracts-core) | Hardhat, Solidity, ERC-4337 | Core marketplace protocol, NFT standards, and Smart Account infrastructure. |
| **API Service** | [api-service](https://github.com/NFT-marketplace-blockchain/api-service) | FastAPI, Python, Web3.py | Off-chain indexer, REST API for data query, and WebSocket gateway. |

### User Interfaces

| Application | Repository | Technologies | Description |
| :--- | :--- | :--- | :--- |
| **Web Client** | [web-client](https://github.com/NFT-marketplace-blockchain/nft-marketplace-admin) | Next.js 15, Wagmi | Primary marketplace interface for trading, collecting, and wallet management. |
| **Admin Portal** | [admin-portal](https://github.com/NFT-marketplace-blockchain/nft-marketplace-app) | Vite, React, Shadcn | Dashboard for platform operations, campaign management, and analytics. |

## System Workflow

1.  **Blockchain Layer**: Assets and Orders are secured on-chain (Sepolia). Account Abstraction allows gasless transactions.
2.  **Indexing Layer**: The **API Service** listens to contract events in real-time, indexing them into a query-optimized database.
3.  **Application Layer**: 
    *   **Web Client** queries the API for fast display and interacts directly with Contracts for execution.
    *   **Admin Portal** manages system configurations and operational data.

## Deployment

The system is currently deployed on the **Sepolia Testnet**.

*   **Network**: Sepolia
*   **Indexer Status**: Active
*   **Contracts**: Deployed & Verified

---
