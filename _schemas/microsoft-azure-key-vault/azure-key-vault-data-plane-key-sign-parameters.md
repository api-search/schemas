---
description: The key sign parameters.
layout: schema
name: KeySignParameters
properties_list:
- description: The signing/verification algorithm identifier.
  name: alg
  type: string
- description: The digest value to sign.
  name: value
  type: string
provider_name: Azure Key Vault
provider_slug: microsoft-azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-key-sign-parameters-schema.json
slug: azure-key-vault-data-plane-key-sign-parameters
source_filename: azure-key-vault-data-plane-key-sign-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeySignParameters\",\n  \"type\": \"object\",\n  \"description\": \"The key sign parameters.\",\n  \"properties\": {\n    \"alg\": {\n      \"type\": \"string\",\n      \"description\": \"The signing/verification algorithm identifier.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The digest value to sign.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-key-sign-parameters-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: KeySignParameters
---
