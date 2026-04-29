---
description: ERC-20 token balance entry for a wallet address.
layout: schema
name: Token Balance
properties_list:
- description: Token contract address.
  name: contractAddress
  type: string
- description: Token balance in hexadecimal (raw units, divide by 10^decimals).
  name: tokenBalance
  type: string
- description: Error message if the balance could not be retrieved.
  name: error
  type: string
provider_name: Alchemy
provider_slug: alchemy
schema_file: json-schema/alchemy-token-api-token-balance-schema.json
slug: alchemy-token-api-token-balance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-token-api-token-balance-schema.json\",\n  \"title\": \"Token Balance\",\n  \"description\": \"ERC-20 token balance entry for a wallet address.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contractAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Token contract address.\",\n      \"example\": \"0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48\"\n    },\n    \"tokenBalance\": {\n      \"type\": \"string\",\n      \"description\": \"Token balance in hexadecimal (raw units, divide by 10^decimals).\",\n      \"example\": \"0x0000000000000000000000000000000000000000000000000de0b6b3a7640000\"\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Error message if the balance could not be retrieved.\",\n      \"example\": null\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-token-api-token-balance-schema.json
tags:
- Blockchain
- Cryptocurrency
- Web3
- Account Abstraction
- Ethereum
title: Token Balance
---
