---
description: The key item containing key metadata.
layout: schema
name: KeyItem
properties_list:
- description: Key identifier.
  name: kid
  type: string
- description: ''
  name: tags
  type: object
- description: ''
  name: managed
  type: boolean
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-key-vault-key-item-schema.json
slug: azure-key-vault-key-item
source_filename: azure-key-vault-key-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyItem\",\n  \"type\": \"object\",\n  \"description\": \"The key item containing key metadata.\",\n  \"properties\": {\n    \"kid\": {\n      \"type\": \"string\",\n      \"description\": \"Key identifier.\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    },\n    \"managed\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-key-vault-key-item-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: KeyItem
---
