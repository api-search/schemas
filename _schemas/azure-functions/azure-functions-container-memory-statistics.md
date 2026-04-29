---
description: ContainerMemoryStatistics schema from Azure Functions API
layout: schema
name: ContainerMemoryStatistics
properties_list:
- description: ''
  name: limit
  type: integer
- description: ''
  name: maxUsage
  type: integer
- description: ''
  name: usage
  type: integer
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-container-memory-statistics-schema.json
slug: azure-functions-container-memory-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-container-memory-statistics-schema.json\",\n  \"title\": \"ContainerMemoryStatistics\",\n  \"description\": \"ContainerMemoryStatistics schema from Azure Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"limit\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"maxUsage\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"usage\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-container-memory-statistics-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: ContainerMemoryStatistics
---
