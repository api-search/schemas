---
description: ContainerMemoryStatistics schema from Azure Function Apps API
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
provider_name: Azure Function Apps
provider_slug: azure-function-apps
schema_file: json-schema/azure-function-apps-container-memory-statistics-schema.json
slug: azure-function-apps-container-memory-statistics
source_filename: azure-function-apps-container-memory-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-container-memory-statistics-schema.json\",\n  \"title\": \"ContainerMemoryStatistics\",\n  \"description\": \"ContainerMemoryStatistics schema from Azure Function Apps API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"limit\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"maxUsage\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"usage\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-container-memory-statistics-schema.json
tags:
- Azure
- Compute
- FaaS
- Functions
- Serverless
title: ContainerMemoryStatistics
---
