---
description: The key verify parameters.
layout: schema
name: KeyVerifyParameters
properties_list:
- description: The signing/verification algorithm identifier.
  name: alg
  type: string
- description: The digest used for signing.
  name: digest
  type: string
- description: The signature to verify.
  name: value
  type: string
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-key-verify-parameters-schema.json
slug: azure-key-vault-data-plane-key-verify-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyVerifyParameters\",\n  \"type\": \"object\",\n  \"description\": \"The key verify parameters.\",\n  \"properties\": {\n    \"alg\": {\n      \"type\": \"string\",\n      \"description\": \"The signing/verification algorithm identifier.\"\n    },\n    \"digest\": {\n      \"type\": \"string\",\n      \"description\": \"The digest used for signing.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The signature to verify.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-key-verify-parameters-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: KeyVerifyParameters
---
