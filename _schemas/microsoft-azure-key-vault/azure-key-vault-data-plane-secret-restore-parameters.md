---
description: The secret restore parameters.
layout: schema
name: SecretRestoreParameters
properties_list:
- description: The backup blob associated with a secret bundle.
  name: value
  type: string
provider_name: Azure Key Vault
provider_slug: microsoft-azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-secret-restore-parameters-schema.json
slug: azure-key-vault-data-plane-secret-restore-parameters
source_filename: azure-key-vault-data-plane-secret-restore-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecretRestoreParameters\",\n  \"type\": \"object\",\n  \"description\": \"The secret restore parameters.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The backup blob associated with a secret bundle.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-secret-restore-parameters-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: SecretRestoreParameters
---
