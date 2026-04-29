---
description: ContainerNetworkInterfaceStatistics schema from Azure Function Apps API
layout: schema
name: ContainerNetworkInterfaceStatistics
properties_list:
- description: ''
  name: rxBytes
  type: integer
- description: ''
  name: rxDropped
  type: integer
- description: ''
  name: rxErrors
  type: integer
- description: ''
  name: rxPackets
  type: integer
- description: ''
  name: txBytes
  type: integer
- description: ''
  name: txDropped
  type: integer
- description: ''
  name: txErrors
  type: integer
- description: ''
  name: txPackets
  type: integer
provider_name: Azure Function Apps
provider_slug: azure-function-apps
schema_file: json-schema/azure-function-apps-container-network-interface-statistics-schema.json
slug: azure-function-apps-container-network-interface-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-container-network-interface-statistics-schema.json\",\n  \"title\": \"ContainerNetworkInterfaceStatistics\",\n  \"description\": \"ContainerNetworkInterfaceStatistics schema from Azure Function Apps API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rxBytes\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"rxDropped\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"rxErrors\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"rxPackets\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"txBytes\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"txDropped\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"\
  txErrors\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"txPackets\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-container-network-interface-statistics-schema.json
tags:
- Azure
- Compute
- FaaS
- Functions
- Serverless
title: ContainerNetworkInterfaceStatistics
---
