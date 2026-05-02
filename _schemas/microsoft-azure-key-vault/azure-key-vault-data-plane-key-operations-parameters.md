---
description: The key operations parameters.
layout: schema
name: KeyOperationsParameters
properties_list:
- description: Algorithm identifier.
  name: alg
  type: string
- description: The value to operate on.
  name: value
  type: string
- description: Initialization vector for symmetric algorithms.
  name: iv
  type: string
- description: Additional data to authenticate but not encrypt/decrypt.
  name: aad
  type: string
- description: The tag to verify when performing decryption with an authenticated algorithm.
  name: tag
  type: string
provider_name: Azure Key Vault
provider_slug: microsoft-azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-key-operations-parameters-schema.json
slug: azure-key-vault-data-plane-key-operations-parameters
source_filename: azure-key-vault-data-plane-key-operations-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyOperationsParameters\",\n  \"type\": \"object\",\n  \"description\": \"The key operations parameters.\",\n  \"properties\": {\n    \"alg\": {\n      \"type\": \"string\",\n      \"description\": \"Algorithm identifier.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value to operate on.\"\n    },\n    \"iv\": {\n      \"type\": \"string\",\n      \"description\": \"Initialization vector for symmetric algorithms.\"\n    },\n    \"aad\": {\n      \"type\": \"string\",\n      \"description\": \"Additional data to authenticate but not encrypt/decrypt.\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"The tag to verify when performing decryption with an authenticated algorithm.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-key-operations-parameters-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: KeyOperationsParameters
---
