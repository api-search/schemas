---
description: JSON-RPC request to sponsor a user operation via the Gas Manager paymaster.
layout: schema
name: Sponsor User Operation Request
properties_list:
- description: Request ID.
  name: id
  type: integer
- description: JSON-RPC version.
  name: jsonrpc
  type: string
- description: Alchemy paymaster method.
  name: method
  type: string
- description: Sponsorship parameters array.
  name: params
  type: array
provider_name: Alchemy
provider_slug: alchemy
schema_file: json-schema/alchemy-gas-manager-api-sponsor-user-operation-request-schema.json
slug: alchemy-gas-manager-api-sponsor-user-operation-request
source_filename: alchemy-gas-manager-api-sponsor-user-operation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-gas-manager-api-sponsor-user-operation-request-schema.json\",\n  \"title\": \"Sponsor User Operation Request\",\n  \"description\": \"JSON-RPC request to sponsor a user operation via the Gas Manager paymaster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Request ID.\",\n      \"example\": 1\n    },\n    \"jsonrpc\": {\n      \"type\": \"string\",\n      \"description\": \"JSON-RPC version.\",\n      \"example\": \"2.0\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"description\": \"Alchemy paymaster method.\",\n      \"example\": \"alchemy_requestGasAndPaymasterAndData\"\n    },\n    \"params\": {\n      \"type\": \"array\",\n      \"description\": \"Sponsorship parameters array.\",\n      \"items\": {}\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-gas-manager-api-sponsor-user-operation-request-schema.json
tags:
- Blockchain
- Cryptocurrency
- Web3
- Account Abstraction
- Ethereum
title: Sponsor User Operation Request
---
