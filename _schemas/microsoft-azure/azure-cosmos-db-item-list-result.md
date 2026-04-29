---
description: List of Cosmos DB items.
layout: schema
name: ItemListResult
properties_list:
- description: ''
  name: _rid
  type: string
- description: List of items.
  name: Documents
  type: array
- description: ''
  name: _count
  type: integer
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cosmos-db-item-list-result-schema.json
slug: azure-cosmos-db-item-list-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ItemListResult\",\n  \"type\": \"object\",\n  \"description\": \"List of Cosmos DB items.\",\n  \"properties\": {\n    \"_rid\": {\n      \"type\": \"string\"\n    },\n    \"Documents\": {\n      \"type\": \"array\",\n      \"description\": \"List of items.\"\n    },\n    \"_count\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cosmos-db-item-list-result-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ItemListResult
---
