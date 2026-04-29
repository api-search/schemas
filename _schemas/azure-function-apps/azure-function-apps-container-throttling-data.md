---
description: ContainerThrottlingData schema from Azure Function Apps API
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
provider_name: Azure Function Apps
provider_slug: azure-function-apps
schema_file: json-schema/azure-function-apps-container-throttling-data-schema.json
slug: azure-function-apps-container-throttling-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-container-throttling-data-schema.json\",\n  \"title\": \"ContainerThrottlingData\",\n  \"description\": \"ContainerThrottlingData schema from Azure Function Apps API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"periods\": {\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"throttledPeriods\": {\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"throttledTime\": {\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-container-throttling-data-schema.json
tags:
- Azure
- Compute
- FaaS
- Functions
- Serverless
title: ContainerThrottlingData
---
