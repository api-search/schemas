---
description: ResourceGroupListResult schema from Microsoft Azure API
layout: schema
name: ResourceGroupListResult
properties_list:
- description: ''
  name: value
  type: array
- description: ''
  name: nextLink
  type: string
provider_name: Microsoft Azure
provider_slug: azure
schema_file: json-schema/azure-resource-group-list-result-schema.json
slug: azure-resource-group-list-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/json-schema/azure-resource-group-list-result-schema.json\",\n  \"title\": \"ResourceGroupListResult\",\n  \"description\": \"ResourceGroupListResult schema from Microsoft Azure API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ResourceGroup\"\n      }\n    },\n    \"nextLink\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/json-schema/azure-resource-group-list-result-schema.json
tags:
- Cloud Computing
- Databases
- Infrastructure
- Machine Learning
- Networking
- Platform as a Service
- Storage
title: ResourceGroupListResult
---
