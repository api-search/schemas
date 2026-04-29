---
description: JSON-RPC response for sponsored user operation requests.
layout: schema
name: Sponsor User Operation Response
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: jsonrpc
  type: string
- description: Paymaster response data for a sponsored user operation.
  name: result
  type: object
provider_name: Alchemy
provider_slug: alchemy
schema_file: json-schema/alchemy-gas-manager-api-sponsor-user-operation-response-schema.json
slug: alchemy-gas-manager-api-sponsor-user-operation-response
source_filename: alchemy-gas-manager-api-sponsor-user-operation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-gas-manager-api-sponsor-user-operation-response-schema.json\",\n  \"title\": \"Sponsor User Operation Response\",\n  \"description\": \"JSON-RPC response for sponsored user operation requests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"jsonrpc\": {\n      \"type\": \"string\",\n      \"example\": \"2.0\"\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"title\": \"Sponsor User Operation Result\",\n      \"description\": \"Paymaster response data for a sponsored user operation.\",\n      \"properties\": {\n        \"paymasterAndData\": {\n          \"type\": \"string\",\n          \"description\": \"Encoded paymaster address and data for the user operation.\",\n          \"example\": \"0xabc123paymaster\"\
  \n        },\n        \"preVerificationGas\": {\n          \"type\": \"string\",\n          \"description\": \"Pre-verification gas estimate in hexadecimal.\",\n          \"example\": \"0x5208\"\n        },\n        \"verificationGasLimit\": {\n          \"type\": \"string\",\n          \"description\": \"Verification gas limit in hexadecimal.\",\n          \"example\": \"0x15f90\"\n        },\n        \"callGasLimit\": {\n          \"type\": \"string\",\n          \"description\": \"Call gas limit in hexadecimal.\",\n          \"example\": \"0x9c40\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-gas-manager-api-sponsor-user-operation-response-schema.json
tags:
- Blockchain
- Cryptocurrency
- Web3
- Account Abstraction
- Ethereum
title: Sponsor User Operation Response
---
