---
description: A secret consisting of a value, id and its attributes.
layout: schema
name: SecretBundle
properties_list:
- description: The secret value.
  name: value
  type: string
- description: The secret id.
  name: id
  type: string
- description: The content type of the secret.
  name: contentType
  type: string
- description: Application specific metadata in the form of key-value pairs.
  name: tags
  type: object
- description: If this is a secret backing a KV certificate, then this field specifies the corresponding key backing the KV certificate.
  name: kid
  type: string
- description: True if the secret's lifetime is managed by key vault. If this is a secret backing a certificate, then managed will be true.
  name: managed
  type: boolean
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-secret-bundle-schema.json
slug: azure-key-vault-data-plane-secret-bundle
source_filename: azure-key-vault-data-plane-secret-bundle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecretBundle\",\n  \"type\": \"object\",\n  \"description\": \"A secret consisting of a value, id and its attributes.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The secret value.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The secret id.\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The content type of the secret.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application specific metadata in the form of key-value pairs.\"\n    },\n    \"kid\": {\n      \"type\": \"string\",\n      \"description\": \"If this is a secret backing a KV certificate, then this field specifies the corresponding key backing the KV certificate.\"\n    },\n    \"managed\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the secret's lifetime\
  \ is managed by key vault. If this is a secret backing a certificate, then managed will be true.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-secret-bundle-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: SecretBundle
---
