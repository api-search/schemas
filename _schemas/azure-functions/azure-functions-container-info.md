---
description: ContainerInfo schema from Azure Functions API
layout: schema
name: ContainerInfo
properties_list:
- description: ''
  name: currentCpuStats
  type: object
- description: ''
  name: currentTimeStamp
  type: string
- description: ''
  name: eth0
  type: object
- description: ''
  name: id
  type: string
- description: ''
  name: memoryStats
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: previousCpuStats
  type: object
- description: ''
  name: previousTimeStamp
  type: string
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-container-info-schema.json
slug: azure-functions-container-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-container-info-schema.json\",\n  \"title\": \"ContainerInfo\",\n  \"description\": \"ContainerInfo schema from Azure Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currentCpuStats\": {\n      \"$ref\": \"#/definitions/ContainerCpuStatistics\"\n    },\n    \"currentTimeStamp\": {\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"eth0\": {\n      \"$ref\": \"#/definitions/ContainerNetworkInterfaceStatistics\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"memoryStats\": {\n      \"$ref\": \"#/definitions/ContainerMemoryStatistics\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"previousCpuStats\": {\n      \"$ref\": \"#/definitions/ContainerCpuStatistics\"\n    },\n    \"previousTimeStamp\": {\n    \
  \  \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-container-info-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: ContainerInfo
---
