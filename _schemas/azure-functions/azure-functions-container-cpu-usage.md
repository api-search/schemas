---
description: ContainerCpuUsage schema from Azure Functions API
layout: schema
name: ContainerCpuUsage
properties_list:
- description: ''
  name: kernelModeUsage
  type: integer
- description: ''
  name: perCpuUsage
  type: array
- description: ''
  name: totalUsage
  type: integer
- description: ''
  name: userModeUsage
  type: integer
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-container-cpu-usage-schema.json
slug: azure-functions-container-cpu-usage
source_filename: azure-functions-container-cpu-usage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-container-cpu-usage-schema.json\",\n  \"title\": \"ContainerCpuUsage\",\n  \"description\": \"ContainerCpuUsage schema from Azure Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kernelModeUsage\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"perCpuUsage\": {\n      \"items\": {\n        \"format\": \"int64\",\n        \"type\": \"integer\"\n      },\n      \"type\": \"array\"\n    },\n    \"totalUsage\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"userModeUsage\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-container-cpu-usage-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: ContainerCpuUsage
---
