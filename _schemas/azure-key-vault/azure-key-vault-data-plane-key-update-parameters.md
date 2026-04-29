---
description: The key update parameters.
layout: schema
name: KeyUpdateParameters
properties_list:
- description: JSON web key operations.
  name: key_ops
  type: array
- description: Application specific metadata in the form of key-value pairs.
  name: tags
  type: object
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-key-update-parameters-schema.json
slug: azure-key-vault-data-plane-key-update-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyUpdateParameters\",\n  \"type\": \"object\",\n  \"description\": \"The key update parameters.\",\n  \"properties\": {\n    \"key_ops\": {\n      \"type\": \"array\",\n      \"description\": \"JSON web key operations.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application specific metadata in the form of key-value pairs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-key-update-parameters-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: KeyUpdateParameters
---
