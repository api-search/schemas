---
description: Paymaster response data for a sponsored user operation.
layout: schema
name: Sponsor User Operation Result
properties_list:
- description: Encoded paymaster address and data for the user operation.
  name: paymasterAndData
  type: string
- description: Pre-verification gas estimate in hexadecimal.
  name: preVerificationGas
  type: string
- description: Verification gas limit in hexadecimal.
  name: verificationGasLimit
  type: string
- description: Call gas limit in hexadecimal.
  name: callGasLimit
  type: string
provider_name: Alchemy
provider_slug: alchemy
schema_file: json-schema/alchemy-gas-manager-api-sponsor-user-operation-result-schema.json
slug: alchemy-gas-manager-api-sponsor-user-operation-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-gas-manager-api-sponsor-user-operation-result-schema.json\",\n  \"title\": \"Sponsor User Operation Result\",\n  \"description\": \"Paymaster response data for a sponsored user operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"paymasterAndData\": {\n      \"type\": \"string\",\n      \"description\": \"Encoded paymaster address and data for the user operation.\",\n      \"example\": \"0xabc123paymaster\"\n    },\n    \"preVerificationGas\": {\n      \"type\": \"string\",\n      \"description\": \"Pre-verification gas estimate in hexadecimal.\",\n      \"example\": \"0x5208\"\n    },\n    \"verificationGasLimit\": {\n      \"type\": \"string\",\n      \"description\": \"Verification gas limit in hexadecimal.\",\n      \"example\": \"0x15f90\"\n    },\n    \"callGasLimit\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Call gas limit in hexadecimal.\",\n      \"example\": \"0x9c40\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-gas-manager-api-sponsor-user-operation-result-schema.json
tags:
- Blockchain
- Cryptocurrency
- Web3
- Account Abstraction
- Ethereum
title: Sponsor User Operation Result
---
