---
description: The key create parameters.
layout: schema
name: KeyCreateParameters
properties_list:
- description: The type of key to create.
  name: kty
  type: string
- description: The key size in bits. For example, 2048, 3072, or 4096 for RSA.
  name: key_size
  type: integer
- description: JSON web key operations.
  name: key_ops
  type: array
- description: Application-specific metadata.
  name: tags
  type: object
- description: Elliptic curve name (for EC key types).
  name: crv
  type: string
- description: Whether the private key can be exported.
  name: exportable
  type: boolean
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-key-vault-key-create-parameters-schema.json
slug: azure-key-vault-key-create-parameters
source_filename: azure-key-vault-key-create-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyCreateParameters\",\n  \"type\": \"object\",\n  \"description\": \"The key create parameters.\",\n  \"properties\": {\n    \"kty\": {\n      \"type\": \"string\",\n      \"description\": \"The type of key to create.\"\n    },\n    \"key_size\": {\n      \"type\": \"integer\",\n      \"description\": \"The key size in bits. For example, 2048, 3072, or 4096 for RSA.\"\n    },\n    \"key_ops\": {\n      \"type\": \"array\",\n      \"description\": \"JSON web key operations.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application-specific metadata.\"\n    },\n    \"crv\": {\n      \"type\": \"string\",\n      \"description\": \"Elliptic curve name (for EC key types).\"\n    },\n    \"exportable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the private key can be exported.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-key-vault-key-create-parameters-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: KeyCreateParameters
---
