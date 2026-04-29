---
description: ContainerThrottlingData schema from Azure Functions API
layout: schema
name: ContainerThrottlingData
properties_list:
- description: ''
  name: periods
  type: integer
- description: ''
  name: throttledPeriods
  type: integer
- description: ''
  name: throttledTime
  type: integer
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-container-throttling-data-schema.json
slug: azure-functions-container-throttling-data
source_filename: azure-functions-container-throttling-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-container-throttling-data-schema.json\",\n  \"title\": \"ContainerThrottlingData\",\n  \"description\": \"ContainerThrottlingData schema from Azure Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"periods\": {\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"throttledPeriods\": {\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"throttledTime\": {\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-container-throttling-data-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: ContainerThrottlingData
---
