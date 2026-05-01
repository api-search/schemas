---
description: A fiat-to-stablecoin, stablecoin-to-fiat, payout, or swap order processed by the Grapes Finance API.
layout: schema
name: Grapes Finance Order
properties_list:
- description: Unique order identifier.
  name: id
  type: string
- description: Type of order being executed.
  name: type
  type: string
- description: Source asset being converted from.
  name: sourceAsset
  type: string
- description: Destination asset being converted to.
  name: destinationAsset
  type: string
- description: Decimal amount represented as a string to preserve precision.
  name: amount
  type: string
- description: Current order processing state.
  name: status
  type: string
- description: Identifier of the user submitting the order.
  name: userId
  type: string
- description: Wallet involved in the order, if applicable.
  name: walletId
  type: string
- description: Beneficiary contact identifier for payouts.
  name: contactId
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: settledAt
  type: string
provider_name: Grapes Finance
provider_slug: grapes-finance
schema_file: json-schema/grapes-finance-order-schema.json
slug: grapes-finance-order
source_filename: grapes-finance-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/grapes-finance/refs/heads/main/json-schema/grapes-finance-order-schema.json\",\n  \"title\": \"Grapes Finance Order\",\n  \"description\": \"A fiat-to-stablecoin, stablecoin-to-fiat, payout, or swap order processed by the Grapes Finance API.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\", \"sourceAsset\", \"destinationAsset\", \"amount\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique order identifier.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"onramp\", \"offramp\", \"payout\", \"swap\"],\n      \"description\": \"Type of order being executed.\"\n    },\n    \"sourceAsset\": {\n      \"type\": \"string\",\n      \"enum\": [\"USDC\", \"QCAD\", \"CAD\", \"USD\"],\n      \"description\": \"Source asset being converted from.\"\n    },\n\
  \    \"destinationAsset\": {\n      \"type\": \"string\",\n      \"enum\": [\"USDC\", \"QCAD\", \"CAD\", \"USD\"],\n      \"description\": \"Destination asset being converted to.\"\n    },\n    \"amount\": {\n      \"type\": \"string\",\n      \"description\": \"Decimal amount represented as a string to preserve precision.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"pending\", \"processing\", \"settled\", \"failed\"],\n      \"description\": \"Current order processing state.\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the user submitting the order.\"\n    },\n    \"walletId\": {\n      \"type\": \"string\",\n      \"description\": \"Wallet involved in the order, if applicable.\"\n    },\n    \"contactId\": {\n      \"type\": \"string\",\n      \"description\": \"Beneficiary contact identifier for payouts.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n\
  \    },\n    \"settledAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/grapes-finance/refs/heads/main/json-schema/grapes-finance-order-schema.json
tags:
- Stablecoin
- Onramp
- Offramp
- Fiat
- Payments
- Cryptocurrency
- Embedded Finance
title: Grapes Finance Order
---
