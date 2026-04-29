---
description: The key vault server error.
layout: schema
name: Error
properties_list:
- description: The error code.
  name: code
  type: string
- description: The error message.
  name: message
  type: string
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-error-schema.json
slug: azure-key-vault-data-plane-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"The key vault server error.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The error code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The error message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-error-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: Error
---
