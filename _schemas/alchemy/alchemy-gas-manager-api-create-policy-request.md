---
description: Request body for creating a new gas manager policy.
layout: schema
name: Create Policy Request
properties_list:
- description: Display name for the new policy.
  name: name
  type: string
- description: Blockchain network for the policy.
  name: network
  type: string
- description: Maximum ETH spend per user (optional).
  name: maxSpendPerUser
  type: number
- description: Maximum total ETH spend across all users (optional).
  name: maxSpendTotal
  type: number
provider_name: Alchemy
provider_slug: alchemy
schema_file: json-schema/alchemy-gas-manager-api-create-policy-request-schema.json
slug: alchemy-gas-manager-api-create-policy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-gas-manager-api-create-policy-request-schema.json\",\n  \"title\": \"Create Policy Request\",\n  \"description\": \"Request body for creating a new gas manager policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the new policy.\",\n      \"example\": \"My Sponsorship Policy\"\n    },\n    \"network\": {\n      \"type\": \"string\",\n      \"description\": \"Blockchain network for the policy.\",\n      \"example\": \"eth-mainnet\"\n    },\n    \"maxSpendPerUser\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Maximum ETH spend per user (optional).\",\n      \"example\": 1.0\n    },\n    \"maxSpendTotal\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n \
  \     \"description\": \"Maximum total ETH spend across all users (optional).\",\n      \"example\": 500.0\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"network\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-gas-manager-api-create-policy-request-schema.json
tags:
- Blockchain
- Cryptocurrency
- Web3
- Account Abstraction
- Ethereum
title: Create Policy Request
---
