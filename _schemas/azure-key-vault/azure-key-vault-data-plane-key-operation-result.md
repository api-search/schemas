---
description: The key operation result.
layout: schema
name: KeyOperationResult
properties_list:
- description: Key identifier.
  name: kid
  type: string
- description: The result of the operation.
  name: value
  type: string
- description: Initialization vector for symmetric algorithms.
  name: iv
  type: string
- description: Authentication tag for authenticated encryption algorithms.
  name: tag
  type: string
- description: Additional authenticated data.
  name: aad
  type: string
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-key-operation-result-schema.json
slug: azure-key-vault-data-plane-key-operation-result
source_filename: azure-key-vault-data-plane-key-operation-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyOperationResult\",\n  \"type\": \"object\",\n  \"description\": \"The key operation result.\",\n  \"properties\": {\n    \"kid\": {\n      \"type\": \"string\",\n      \"description\": \"Key identifier.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The result of the operation.\"\n    },\n    \"iv\": {\n      \"type\": \"string\",\n      \"description\": \"Initialization vector for symmetric algorithms.\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication tag for authenticated encryption algorithms.\"\n    },\n    \"aad\": {\n      \"type\": \"string\",\n      \"description\": \"Additional authenticated data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-key-operation-result-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: KeyOperationResult
---
