---
description: Represents a Binance user account with balances, permissions, and commission rates.
layout: schema
name: Binance Account
properties_list:
- description: Maker commission rate in basis points.
  name: makerCommission
  type: integer
- description: Taker commission rate in basis points.
  name: takerCommission
  type: integer
- description: Buyer commission rate in basis points.
  name: buyerCommission
  type: integer
- description: Seller commission rate in basis points.
  name: sellerCommission
  type: integer
- description: Detailed commission rate structure.
  name: commissionRates
  type: object
- description: Whether the account has trading permission.
  name: canTrade
  type: boolean
- description: Whether the account has withdrawal permission.
  name: canWithdraw
  type: boolean
- description: Whether the account has deposit permission.
  name: canDeposit
  type: boolean
- description: Whether this is a brokered account.
  name: brokered
  type: boolean
- description: Whether self-trade prevention is required.
  name: requireSelfTradePrevention
  type: boolean
- description: Whether Smart Order Routing is prevented.
  name: preventSor
  type: boolean
- description: Last account update time in milliseconds since epoch.
  name: updateTime
  type: integer
- description: Account type identifier.
  name: accountType
  type: string
- description: List of asset balances in the account.
  name: balances
  type: array
- description: Account permission types.
  name: permissions
  type: array
- description: Unique user identifier.
  name: uid
  type: integer
provider_name: Binance
provider_slug: binance
schema_file: json-schema/binance-account-schema.json
slug: binance-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/binance/account.json\",\n  \"title\": \"Binance Account\",\n  \"description\": \"Represents a Binance user account with balances, permissions, and commission rates.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"makerCommission\": {\n      \"type\": \"integer\",\n      \"description\": \"Maker commission rate in basis points.\"\n    },\n    \"takerCommission\": {\n      \"type\": \"integer\",\n      \"description\": \"Taker commission rate in basis points.\"\n    },\n    \"buyerCommission\": {\n      \"type\": \"integer\",\n      \"description\": \"Buyer commission rate in basis points.\"\n    },\n    \"sellerCommission\": {\n      \"type\": \"integer\",\n      \"description\": \"Seller commission rate in basis points.\"\n    },\n    \"commissionRates\": {\n      \"type\": \"object\",\n      \"description\": \"Detailed commission rate structure.\",\n\
  \      \"properties\": {\n        \"maker\": {\n          \"type\": \"string\",\n          \"description\": \"Maker rate as decimal string.\"\n        },\n        \"taker\": {\n          \"type\": \"string\",\n          \"description\": \"Taker rate as decimal string.\"\n        },\n        \"buyer\": {\n          \"type\": \"string\",\n          \"description\": \"Buyer rate as decimal string.\"\n        },\n        \"seller\": {\n          \"type\": \"string\",\n          \"description\": \"Seller rate as decimal string.\"\n        }\n      }\n    },\n    \"canTrade\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account has trading permission.\"\n    },\n    \"canWithdraw\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account has withdrawal permission.\"\n    },\n    \"canDeposit\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account has deposit permission.\"\n    },\n    \"brokered\": {\n      \"type\": \"\
  boolean\",\n      \"description\": \"Whether this is a brokered account.\"\n    },\n    \"requireSelfTradePrevention\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether self-trade prevention is required.\"\n    },\n    \"preventSor\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Smart Order Routing is prevented.\"\n    },\n    \"updateTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Last account update time in milliseconds since epoch.\"\n    },\n    \"accountType\": {\n      \"type\": \"string\",\n      \"description\": \"Account type identifier.\",\n      \"enum\": [\"SPOT\", \"MARGIN\", \"FUTURES\"]\n    },\n    \"balances\": {\n      \"type\": \"array\",\n      \"description\": \"List of asset balances in the account.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Balance\"\n      }\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n      \"description\": \"Account permission types.\"\
  ,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"uid\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unique user identifier.\"\n    }\n  },\n  \"$defs\": {\n    \"Balance\": {\n      \"type\": \"object\",\n      \"description\": \"Asset balance within an account.\",\n      \"required\": [\"asset\", \"free\", \"locked\"],\n      \"properties\": {\n        \"asset\": {\n          \"type\": \"string\",\n          \"description\": \"Asset symbol, e.g. BTC, USDT.\",\n          \"pattern\": \"^[A-Z0-9]+$\"\n        },\n        \"free\": {\n          \"type\": \"string\",\n          \"description\": \"Available balance for trading and withdrawal.\",\n          \"pattern\": \"^\\\\d+\\\\.?\\\\d*$\"\n        },\n        \"locked\": {\n          \"type\": \"string\",\n          \"description\": \"Balance locked in open orders or pending operations.\",\n          \"pattern\": \"^\\\\d+\\\\.?\\\\d*$\"\n        }\n      }\n    }\n\
  \  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/json-schema/binance-account-schema.json
tags:
- Cryptocurrency
- Exchange
- Trading
- Blockchain
- Finance
- DeFi
- Market Data
title: Binance Account
---
