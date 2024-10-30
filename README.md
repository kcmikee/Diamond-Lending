# NFT Collateralized Lending Protocol

=====================================

## Overview

This is an open-source implementation of a decentralized lending protocol that utilizes NFTs as collateral. The protocol is designed to facilitate peer-to-peer lending, enabling users to borrow and lend assets in a trustless and secure manner.

## Getting Started

### Installation

1. Clone this repository to your local machine.
2. Install dependencies by running the following command:

```bash
$ yarn && forge update
```

### Compilation

Compile the smart contracts using Hardhat:

```bash
$ npx hardhat compile
```

### Deployment

Deploy the protocol using either Hardhat or Foundry:

#### Hardhat

```bash
$ npx hardhat run scripts/deploy.js
```

#### Foundry

```bash
$ forge t
```

## Notable Features

- The `DiamondLoupeFacet` contract utilizes an updated `LibDiamond` library, which employs Solidity custom errors for improved debugging and diamond upgrades.
- Take a closer look at the `DiamondLoupeFacet` contract in `contracts/facets/DiamondLoupeFacet.sol` and explore the benefits of using custom errors in your own projects!

This protocol uses a Peer-to-Protocol architecture

![Screenshot from 2024-10-30 01-06-32](https://github.com/user-attachments/assets/1efe8e0e-cf0d-40db-a496-e4116ee66561)
