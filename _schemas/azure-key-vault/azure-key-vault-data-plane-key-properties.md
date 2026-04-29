---
description: Properties of the key pair backing a certificate.
layout: schema
name: KeyProperties
properties_list:
- description: Indicates if the private key can be exported.
  name: exportable
  type: boolean
- description: 'The key size in bits. For example: 2048, 3072, or 4096 for RSA.'
  name: key_size
  type: integer
- description: Indicates if the same key pair will be used on certificate renewal.
  name: reuse_key
  type: boolean
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-key-properties-schema.json
slug: azure-key-vault-data-plane-key-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties of the key pair backing a certificate.\",\n  \"properties\": {\n    \"exportable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the private key can be exported.\"\n    },\n    \"key_size\": {\n      \"type\": \"integer\",\n      \"description\": \"The key size in bits. For example: 2048, 3072, or 4096 for RSA.\"\n    },\n    \"reuse_key\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the same key pair will be used on certificate renewal.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-key-properties-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: KeyProperties
---
