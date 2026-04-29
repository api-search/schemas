---
description: The secret item containing secret metadata.
layout: schema
name: SecretItem
properties_list:
- description: Secret identifier.
  name: id
  type: string
- description: ''
  name: tags
  type: object
- description: ''
  name: contentType
  type: string
- description: ''
  name: managed
  type: boolean
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-key-vault-secret-item-schema.json
slug: azure-key-vault-secret-item
source_filename: azure-key-vault-secret-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecretItem\",\n  \"type\": \"object\",\n  \"description\": \"The secret item containing secret metadata.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Secret identifier.\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    },\n    \"contentType\": {\n      \"type\": \"string\"\n    },\n    \"managed\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-key-vault-secret-item-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: SecretItem
---
