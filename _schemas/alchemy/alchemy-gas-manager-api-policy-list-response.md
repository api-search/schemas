---
description: List of gas manager policies.
layout: schema
name: Policy List Response
properties_list:
- description: Array of policy objects.
  name: policies
  type: array
provider_name: Alchemy
provider_slug: alchemy
schema_file: json-schema/alchemy-gas-manager-api-policy-list-response-schema.json
slug: alchemy-gas-manager-api-policy-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-gas-manager-api-policy-list-response-schema.json\",\n  \"title\": \"Policy List Response\",\n  \"description\": \"List of gas manager policies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policies\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"title\": \"Gas Manager Policy\",\n        \"description\": \"A gas sponsorship policy defining rules for covering user operation gas fees.\",\n        \"properties\": {\n          \"policyId\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the policy.\",\n            \"example\": \"pol-abc123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Display name for the policy.\",\n            \"example\": \"Default\
  \ Sponsorship Policy\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"active\",\n              \"inactive\",\n              \"expired\"\n            ],\n            \"description\": \"Current status of the policy.\",\n            \"example\": \"active\"\n          },\n          \"network\": {\n            \"type\": \"string\",\n            \"description\": \"Blockchain network the policy applies to.\",\n            \"example\": \"eth-mainnet\"\n          },\n          \"maxSpendPerUser\": {\n            \"type\": \"number\",\n            \"format\": \"double\",\n            \"description\": \"Maximum ETH spend per user address covered by this policy.\",\n            \"example\": 1.0\n          },\n          \"maxSpendTotal\": {\n            \"type\": \"number\",\n            \"format\": \"double\",\n            \"description\": \"Maximum total ETH spend across all users for this policy.\",\n            \"example\": 1000.0\n\
  \          }\n        }\n      },\n      \"description\": \"Array of policy objects.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-gas-manager-api-policy-list-response-schema.json
tags:
- Blockchain
- Cryptocurrency
- Web3
- Account Abstraction
- Ethereum
title: Policy List Response
---
