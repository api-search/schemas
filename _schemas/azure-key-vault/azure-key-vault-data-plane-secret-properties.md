---
description: Properties of the secret backing a certificate.
layout: schema
name: SecretProperties
properties_list:
- description: The media type (MIME type).
  name: contentType
  type: string
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-secret-properties-schema.json
slug: azure-key-vault-data-plane-secret-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecretProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties of the secret backing a certificate.\",\n  \"properties\": {\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The media type (MIME type).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-secret-properties-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: SecretProperties
---
