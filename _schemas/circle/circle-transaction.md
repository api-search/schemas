---
description: A Circle on-chain transaction record across wallets, smart contracts, and CCTP transfers.
layout: schema
name: Circle Transaction
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: blockchain
  type: string
- description: ''
  name: tokenId
  type: string
- description: ''
  name: walletId
  type: string
- description: ''
  name: sourceAddress
  type: string
- description: ''
  name: destinationAddress
  type: string
- description: ''
  name: transactionType
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: amounts
  type: array
- description: ''
  name: txHash
  type: string
- description: ''
  name: blockHash
  type: string
- description: ''
  name: blockHeight
  type: integer
- description: ''
  name: networkFee
  type: string
- description: ''
  name: estimatedFee
  type: object
- description: ''
  name: errorReason
  type: string
- description: ''
  name: createDate
  type: string
- description: ''
  name: updateDate
  type: string
provider_name: Circle
provider_slug: circle
schema_file: json-schema/circle-transaction-schema.json
slug: circle-transaction
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
title: Circle Transaction
---
