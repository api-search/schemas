---
description: A Circle programmable wallet (developer- or user-controlled) created via the Web3 Services platform.
layout: schema
name: Circle Wallet
properties_list:
- description: Circle-assigned unique identifier for the wallet.
  name: id
  type: string
- description: Public on-chain address for the wallet.
  name: address
  type: string
- description: Blockchain network the wallet is provisioned on.
  name: blockchain
  type: string
- description: Externally Owned Account (EOA) or Smart Contract Account (SCA).
  name: accountType
  type: string
- description: Whether the developer or end user controls the keys.
  name: custodyType
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: walletSetId
  type: string
- description: ''
  name: name
  type: string
- description: Optional client-supplied reference identifier.
  name: refId
  type: string
- description: ''
  name: createDate
  type: string
- description: ''
  name: updateDate
  type: string
provider_name: Circle
provider_slug: circle
schema_file: json-schema/circle-wallet-schema.json
slug: circle-wallet
tags:
- Blockchain
- Compliance
- Cross-Chain
- Currency
- Money
- Payments
- Stablecoin
- Transfers
- USDC
- Wallets
title: Circle Wallet
---
