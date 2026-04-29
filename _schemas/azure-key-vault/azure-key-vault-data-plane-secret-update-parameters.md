---
description: The secret update parameters.
layout: schema
name: SecretUpdateParameters
properties_list:
- description: Type of the secret value such as a password.
  name: contentType
  type: string
- description: Application specific metadata in the form of key-value pairs.
  name: tags
  type: object
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-secret-update-parameters-schema.json
slug: azure-key-vault-data-plane-secret-update-parameters
source_filename: azure-key-vault-data-plane-secret-update-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecretUpdateParameters\",\n  \"type\": \"object\",\n  \"description\": \"The secret update parameters.\",\n  \"properties\": {\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the secret value such as a password.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application specific metadata in the form of key-value pairs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-secret-update-parameters-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: SecretUpdateParameters
---
