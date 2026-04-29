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
source_filename: circle-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/circle/main/json-schema/circle-transaction-schema.json\",\n  \"title\": \"Circle Transaction\",\n  \"description\": \"A Circle on-chain transaction record across wallets, smart contracts, and CCTP transfers.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"blockchain\", \"transactionType\", \"state\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"blockchain\": {\n      \"type\": \"string\"\n    },\n    \"tokenId\": {\n      \"type\": \"string\"\n    },\n    \"walletId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"sourceAddress\": {\n      \"type\": \"string\"\n    },\n    \"destinationAddress\": {\n      \"type\": \"string\"\n    },\n    \"transactionType\": {\n      \"type\": \"string\",\n      \"enum\": [\"INBOUND\", \"OUTBOUND\", \"CONTRACT_DEPLOYMENT\"\
  , \"CONTRACT_EXECUTION\"]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"INITIATED\", \"QUEUED\", \"SENT\", \"CONFIRMED\", \"COMPLETE\", \"FAILED\", \"CANCELLED\", \"DENIED\"]\n    },\n    \"amounts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"txHash\": {\n      \"type\": \"string\"\n    },\n    \"blockHash\": {\n      \"type\": \"string\"\n    },\n    \"blockHeight\": {\n      \"type\": \"integer\",\n      \"minimum\": 0\n    },\n    \"networkFee\": {\n      \"type\": \"string\"\n    },\n    \"estimatedFee\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"gasLimit\": { \"type\": \"string\" },\n        \"baseFee\": { \"type\": \"string\" },\n        \"priorityFee\": { \"type\": \"string\" },\n        \"maxFee\": { \"type\": \"string\" }\n      }\n    },\n    \"errorReason\": {\n      \"type\": \"string\"\n    },\n    \"createDate\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\"\n    },\n    \"updateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/circle/refs/heads/main/json-schema/circle-transaction-schema.json
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
