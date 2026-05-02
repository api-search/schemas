---
description: The key verify result.
layout: schema
name: KeyVerifyResult
properties_list:
- description: True if the signature is verified, otherwise false.
  name: value
  type: boolean
provider_name: Azure Key Vault
provider_slug: microsoft-azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-key-verify-result-schema.json
slug: azure-key-vault-data-plane-key-verify-result
source_filename: azure-key-vault-data-plane-key-verify-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyVerifyResult\",\n  \"type\": \"object\",\n  \"description\": \"The key verify result.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the signature is verified, otherwise false.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-key-verify-result-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: KeyVerifyResult
---
