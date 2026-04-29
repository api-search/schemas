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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/circle/main/json-schema/circle-wallet-schema.json\",\n  \"title\": \"Circle Wallet\",\n  \"description\": \"A Circle programmable wallet (developer- or user-controlled) created via the Web3 Services platform.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"address\", \"blockchain\", \"accountType\", \"custodyType\", \"state\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Circle-assigned unique identifier for the wallet.\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Public on-chain address for the wallet.\"\n    },\n    \"blockchain\": {\n      \"type\": \"string\",\n      \"enum\": [\"ETH\", \"ETH-SEPOLIA\", \"MATIC\", \"MATIC-AMOY\", \"AVAX\", \"AVAX-FUJI\", \"ARB\", \"ARB-SEPOLIA\", \"BASE\", \"BASE-SEPOLIA\", \"SOL\", \"\
  SOL-DEVNET\", \"NEAR\", \"NEAR-TESTNET\"],\n      \"description\": \"Blockchain network the wallet is provisioned on.\"\n    },\n    \"accountType\": {\n      \"type\": \"string\",\n      \"enum\": [\"EOA\", \"SCA\"],\n      \"description\": \"Externally Owned Account (EOA) or Smart Contract Account (SCA).\"\n    },\n    \"custodyType\": {\n      \"type\": \"string\",\n      \"enum\": [\"DEVELOPER\", \"ENDUSER\"],\n      \"description\": \"Whether the developer or end user controls the keys.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"LIVE\", \"FROZEN\"]\n    },\n    \"walletSetId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"refId\": {\n      \"type\": \"string\",\n      \"description\": \"Optional client-supplied reference identifier.\"\n    },\n    \"createDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updateDate\": {\n      \"\
  type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/circle/refs/heads/main/json-schema/circle-wallet-schema.json
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
