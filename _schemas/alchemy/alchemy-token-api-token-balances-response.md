---
description: JSON-RPC response containing token balance results.
layout: schema
name: Token Balances Response
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: jsonrpc
  type: string
- description: Result payload for token balance queries.
  name: result
  type: object
provider_name: Alchemy
provider_slug: alchemy
schema_file: json-schema/alchemy-token-api-token-balances-response-schema.json
slug: alchemy-token-api-token-balances-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-token-api-token-balances-response-schema.json\",\n  \"title\": \"Token Balances Response\",\n  \"description\": \"JSON-RPC response containing token balance results.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"jsonrpc\": {\n      \"type\": \"string\",\n      \"example\": \"2.0\"\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"title\": \"Token Balances Result\",\n      \"description\": \"Result payload for token balance queries.\",\n      \"properties\": {\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Wallet address queried.\",\n          \"example\": \"0x2791bca1f2de4661ed88a30c99a7a9449aa84174\"\n        },\n        \"tokenBalances\": {\n          \"type\": \"\
  array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"title\": \"Token Balance\",\n            \"description\": \"ERC-20 token balance entry for a wallet address.\",\n            \"properties\": {\n              \"contractAddress\": {\n                \"type\": \"string\",\n                \"description\": \"Token contract address.\",\n                \"example\": \"0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48\"\n              },\n              \"tokenBalance\": {\n                \"type\": \"string\",\n                \"description\": \"Token balance in hexadecimal (raw units, divide by 10^decimals).\",\n                \"example\": \"0x0000000000000000000000000000000000000000000000000de0b6b3a7640000\"\n              },\n              \"error\": {\n                \"type\": \"string\",\n                \"nullable\": true,\n                \"description\": \"Error message if the balance could not be retrieved.\",\n                \"example\": null\n         \
  \     }\n            }\n          },\n          \"description\": \"List of token balances for the wallet.\"\n        },\n        \"pageKey\": {\n          \"type\": \"string\",\n          \"nullable\": true,\n          \"description\": \"Pagination key for fetching the next page.\",\n          \"example\": null\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-token-api-token-balances-response-schema.json
tags:
- Blockchain
- Cryptocurrency
- Web3
- Account Abstraction
- Ethereum
title: Token Balances Response
---
