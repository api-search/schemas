---
description: ERC-20 token metadata including name, symbol, decimals, and logo.
layout: schema
name: Token Metadata
properties_list:
- description: Full token name.
  name: name
  type: string
- description: Token ticker symbol.
  name: symbol
  type: string
- description: Number of decimal places for the token.
  name: decimals
  type: integer
- description: URL of the token logo image.
  name: logo
  type: string
provider_name: Alchemy
provider_slug: alchemy
schema_file: json-schema/alchemy-token-api-token-metadata-schema.json
slug: alchemy-token-api-token-metadata
source_filename: alchemy-token-api-token-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-token-api-token-metadata-schema.json\",\n  \"title\": \"Token Metadata\",\n  \"description\": \"ERC-20 token metadata including name, symbol, decimals, and logo.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full token name.\",\n      \"example\": \"USD Coin\"\n    },\n    \"symbol\": {\n      \"type\": \"string\",\n      \"description\": \"Token ticker symbol.\",\n      \"example\": \"USDC\"\n    },\n    \"decimals\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of decimal places for the token.\",\n      \"example\": 6\n    },\n    \"logo\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the token logo image.\",\n      \"example\": \"https://static.alchemyapi.io/images/assets/3408.png\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-token-api-token-metadata-schema.json
tags:
- Blockchain
- Cryptocurrency
- Web3
- Account Abstraction
- Ethereum
title: Token Metadata
---
