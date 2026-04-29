---
description: JSON-RPC response containing token metadata.
layout: schema
name: Token Metadata Response
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: jsonrpc
  type: string
- description: ERC-20 token metadata including name, symbol, decimals, and logo.
  name: result
  type: object
provider_name: Alchemy
provider_slug: alchemy
schema_file: json-schema/alchemy-token-api-token-metadata-response-schema.json
slug: alchemy-token-api-token-metadata-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-token-api-token-metadata-response-schema.json\",\n  \"title\": \"Token Metadata Response\",\n  \"description\": \"JSON-RPC response containing token metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"jsonrpc\": {\n      \"type\": \"string\",\n      \"example\": \"2.0\"\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"title\": \"Token Metadata\",\n      \"description\": \"ERC-20 token metadata including name, symbol, decimals, and logo.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Full token name.\",\n          \"example\": \"USD Coin\"\n        },\n        \"symbol\": {\n          \"type\": \"string\",\n          \"description\": \"\
  Token ticker symbol.\",\n          \"example\": \"USDC\"\n        },\n        \"decimals\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of decimal places for the token.\",\n          \"example\": 6\n        },\n        \"logo\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the token logo image.\",\n          \"example\": \"https://static.alchemyapi.io/images/assets/3408.png\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-token-api-token-metadata-response-schema.json
tags:
- Blockchain
- Cryptocurrency
- Web3
- Account Abstraction
- Ethereum
title: Token Metadata Response
---
