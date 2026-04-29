---
description: ContainerCpuUsage schema from Azure Function Apps API
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
provider_name: Azure Function Apps
provider_slug: azure-function-apps
schema_file: json-schema/azure-function-apps-container-cpu-usage-schema.json
slug: azure-function-apps-container-cpu-usage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-container-cpu-usage-schema.json\",\n  \"title\": \"ContainerCpuUsage\",\n  \"description\": \"ContainerCpuUsage schema from Azure Function Apps API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kernelModeUsage\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"perCpuUsage\": {\n      \"items\": {\n        \"format\": \"int64\",\n        \"type\": \"integer\"\n      },\n      \"type\": \"array\"\n    },\n    \"totalUsage\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"userModeUsage\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-container-cpu-usage-schema.json
tags:
- Azure
- Compute
- FaaS
- Functions
- Serverless
title: ContainerCpuUsage
---
