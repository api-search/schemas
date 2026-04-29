---
description: The secret item containing secret metadata.
layout: schema
name: SecretItem
properties_list:
- description: Secret identifier.
  name: id
  type: string
- description: Application specific metadata in the form of key-value pairs.
  name: tags
  type: object
- description: Type of the secret value such as a password.
  name: contentType
  type: string
- description: True if the secret's lifetime is managed by key vault.
  name: managed
  type: boolean
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-secret-item-schema.json
slug: azure-key-vault-data-plane-secret-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecretItem\",\n  \"type\": \"object\",\n  \"description\": \"The secret item containing secret metadata.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Secret identifier.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application specific metadata in the form of key-value pairs.\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the secret value such as a password.\"\n    },\n    \"managed\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the secret's lifetime is managed by key vault.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-secret-item-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: SecretItem
---
