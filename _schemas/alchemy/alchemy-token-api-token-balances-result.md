---
description: Result payload for token balance queries.
layout: schema
name: Token Balances Result
properties_list:
- description: Wallet address queried.
  name: address
  type: string
- description: List of token balances for the wallet.
  name: tokenBalances
  type: array
- description: Pagination key for fetching the next page.
  name: pageKey
  type: string
provider_name: Alchemy
provider_slug: alchemy
schema_file: json-schema/alchemy-token-api-token-balances-result-schema.json
slug: alchemy-token-api-token-balances-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-token-api-token-balances-result-schema.json\",\n  \"title\": \"Token Balances Result\",\n  \"description\": \"Result payload for token balance queries.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Wallet address queried.\",\n      \"example\": \"0x2791bca1f2de4661ed88a30c99a7a9449aa84174\"\n    },\n    \"tokenBalances\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"title\": \"Token Balance\",\n        \"description\": \"ERC-20 token balance entry for a wallet address.\",\n        \"properties\": {\n          \"contractAddress\": {\n            \"type\": \"string\",\n            \"description\": \"Token contract address.\",\n            \"example\": \"0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48\"\
  \n          },\n          \"tokenBalance\": {\n            \"type\": \"string\",\n            \"description\": \"Token balance in hexadecimal (raw units, divide by 10^decimals).\",\n            \"example\": \"0x0000000000000000000000000000000000000000000000000de0b6b3a7640000\"\n          },\n          \"error\": {\n            \"type\": \"string\",\n            \"nullable\": true,\n            \"description\": \"Error message if the balance could not be retrieved.\",\n            \"example\": null\n          }\n        }\n      },\n      \"description\": \"List of token balances for the wallet.\"\n    },\n    \"pageKey\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Pagination key for fetching the next page.\",\n      \"example\": null\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-token-api-token-balances-result-schema.json
tags:
- Blockchain
- Cryptocurrency
- Web3
- Account Abstraction
- Ethereum
title: Token Balances Result
---
