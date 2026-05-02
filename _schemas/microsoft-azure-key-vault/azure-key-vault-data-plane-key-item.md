---
description: The key item containing key metadata.
layout: schema
name: KeyItem
properties_list:
- description: Key identifier.
  name: kid
  type: string
- description: Application specific metadata in the form of key-value pairs.
  name: tags
  type: object
- description: True if the key's lifetime is managed by key vault.
  name: managed
  type: boolean
provider_name: Azure Key Vault
provider_slug: microsoft-azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-key-item-schema.json
slug: azure-key-vault-data-plane-key-item
source_filename: azure-key-vault-data-plane-key-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyItem\",\n  \"type\": \"object\",\n  \"description\": \"The key item containing key metadata.\",\n  \"properties\": {\n    \"kid\": {\n      \"type\": \"string\",\n      \"description\": \"Key identifier.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application specific metadata in the form of key-value pairs.\"\n    },\n    \"managed\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the key's lifetime is managed by key vault.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-key-item-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: KeyItem
---
