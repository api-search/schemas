---
description: A secret consisting of a value, id, and attributes.
layout: schema
name: SecretBundle
properties_list:
- description: The secret value.
  name: value
  type: string
- description: The secret identifier.
  name: id
  type: string
- description: The content type of the secret.
  name: contentType
  type: string
- description: Application-specific metadata.
  name: tags
  type: object
- description: If the secret is backing a KV certificate, then this field specifies the corresponding key backing the certificate.
  name: kid
  type: string
- description: Whether the secret's lifetime is managed by Key Vault.
  name: managed
  type: boolean
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-key-vault-secret-bundle-schema.json
slug: azure-key-vault-secret-bundle
source_filename: azure-key-vault-secret-bundle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecretBundle\",\n  \"type\": \"object\",\n  \"description\": \"A secret consisting of a value, id, and attributes.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The secret value.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The secret identifier.\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The content type of the secret.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application-specific metadata.\"\n    },\n    \"kid\": {\n      \"type\": \"string\",\n      \"description\": \"If the secret is backing a KV certificate, then this field specifies the corresponding key backing the certificate.\"\n    },\n    \"managed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the secret's lifetime is managed by Key Vault.\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-key-vault-secret-bundle-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: SecretBundle
---
