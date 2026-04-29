---
description: ContainerInfo schema from Azure Function Apps API
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
provider_name: Azure Function Apps
provider_slug: azure-function-apps
schema_file: json-schema/azure-function-apps-container-info-schema.json
slug: azure-function-apps-container-info
source_filename: azure-function-apps-container-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-container-info-schema.json\",\n  \"title\": \"ContainerInfo\",\n  \"description\": \"ContainerInfo schema from Azure Function Apps API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currentCpuStats\": {\n      \"$ref\": \"#/definitions/ContainerCpuStatistics\"\n    },\n    \"currentTimeStamp\": {\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"eth0\": {\n      \"$ref\": \"#/definitions/ContainerNetworkInterfaceStatistics\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"memoryStats\": {\n      \"$ref\": \"#/definitions/ContainerMemoryStatistics\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"previousCpuStats\": {\n      \"$ref\": \"#/definitions/ContainerCpuStatistics\"\n    },\n    \"previousTimeStamp\"\
  : {\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-container-info-schema.json
tags:
- Azure
- Compute
- FaaS
- Functions
- Serverless
title: ContainerInfo
---
