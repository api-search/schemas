---
description: The key create parameters.
layout: schema
name: KeyCreateParameters
properties_list:
- description: 'The key size in bits. For example: 2048, 3072, or 4096 for RSA.'
  name: key_size
  type: integer
- description: The public exponent for a RSA key.
  name: public_exponent
  type: integer
- description: JSON web key operations.
  name: key_ops
  type: array
- description: Application specific metadata in the form of key-value pairs.
  name: tags
  type: object
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-key-create-parameters-schema.json
slug: azure-key-vault-data-plane-key-create-parameters
source_filename: azure-key-vault-data-plane-key-create-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyCreateParameters\",\n  \"type\": \"object\",\n  \"description\": \"The key create parameters.\",\n  \"properties\": {\n    \"key_size\": {\n      \"type\": \"integer\",\n      \"description\": \"The key size in bits. For example: 2048, 3072, or 4096 for RSA.\"\n    },\n    \"public_exponent\": {\n      \"type\": \"integer\",\n      \"description\": \"The public exponent for a RSA key.\"\n    },\n    \"key_ops\": {\n      \"type\": \"array\",\n      \"description\": \"JSON web key operations.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application specific metadata in the form of key-value pairs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-key-create-parameters-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: KeyCreateParameters
---
