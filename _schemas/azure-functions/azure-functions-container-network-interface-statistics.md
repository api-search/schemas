---
description: ContainerNetworkInterfaceStatistics schema from Azure Functions API
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
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-container-network-interface-statistics-schema.json
slug: azure-functions-container-network-interface-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-container-network-interface-statistics-schema.json\",\n  \"title\": \"ContainerNetworkInterfaceStatistics\",\n  \"description\": \"ContainerNetworkInterfaceStatistics schema from Azure Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rxBytes\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"rxDropped\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"rxErrors\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"rxPackets\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"txBytes\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"txDropped\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"txErrors\": {\n\
  \      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"txPackets\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-container-network-interface-statistics-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: ContainerNetworkInterfaceStatistics
---
