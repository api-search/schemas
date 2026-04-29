---
description: The backup secret result, containing the backup blob.
layout: schema
name: BackupSecretResult
properties_list:
- description: The backup blob containing the backed up secret.
  name: value
  type: string
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-backup-secret-result-schema.json
slug: azure-key-vault-data-plane-backup-secret-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BackupSecretResult\",\n  \"type\": \"object\",\n  \"description\": \"The backup secret result, containing the backup blob.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The backup blob containing the backed up secret.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-backup-secret-result-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: BackupSecretResult
---
