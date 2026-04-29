---
description: ContainerCpuStatistics schema from Azure Functions API
layout: schema
name: ContainerCpuStatistics
properties_list:
- description: ''
  name: cpuUsage
  type: object
- description: ''
  name: onlineCpuCount
  type: integer
- description: ''
  name: systemCpuUsage
  type: integer
- description: ''
  name: throttlingData
  type: object
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-container-cpu-statistics-schema.json
slug: azure-functions-container-cpu-statistics
source_filename: azure-functions-container-cpu-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-container-cpu-statistics-schema.json\",\n  \"title\": \"ContainerCpuStatistics\",\n  \"description\": \"ContainerCpuStatistics schema from Azure Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cpuUsage\": {\n      \"$ref\": \"#/definitions/ContainerCpuUsage\"\n    },\n    \"onlineCpuCount\": {\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"systemCpuUsage\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"throttlingData\": {\n      \"$ref\": \"#/definitions/ContainerThrottlingData\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-container-cpu-statistics-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: ContainerCpuStatistics
---
