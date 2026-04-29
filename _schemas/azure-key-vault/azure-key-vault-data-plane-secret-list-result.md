---
description: The secret list result.
layout: schema
name: SecretListResult
properties_list:
- description: A list of secrets.
  name: value
  type: array
- description: The URL to get the next set of secrets.
  name: nextLink
  type: string
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-secret-list-result-schema.json
slug: azure-key-vault-data-plane-secret-list-result
source_filename: azure-key-vault-data-plane-secret-list-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecretListResult\",\n  \"type\": \"object\",\n  \"description\": \"The secret list result.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"A list of secrets.\"\n    },\n    \"nextLink\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to get the next set of secrets.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-secret-list-result-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: SecretListResult
---
