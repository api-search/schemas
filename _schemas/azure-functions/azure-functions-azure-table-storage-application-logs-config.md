---
description: Application logs to Azure table storage configuration.
layout: schema
name: AzureTableStorageApplicationLogsConfig
properties_list:
- description: Log level.
  name: level
  type: string
- description: SAS URL to an Azure table with add/query/delete permissions.
  name: sasUrl
  type: string
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-azure-table-storage-application-logs-config-schema.json
slug: azure-functions-azure-table-storage-application-logs-config
source_filename: azure-functions-azure-table-storage-application-logs-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-azure-table-storage-application-logs-config-schema.json\",\n  \"title\": \"AzureTableStorageApplicationLogsConfig\",\n  \"description\": \"Application logs to Azure table storage configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"level\": {\n      \"description\": \"Log level.\",\n      \"enum\": [\n        \"Off\",\n        \"Verbose\",\n        \"Information\",\n        \"Warning\",\n        \"Error\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"LogLevel\"\n      }\n    },\n    \"sasUrl\": {\n      \"description\": \"SAS URL to an Azure table with add/query/delete permissions.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"sasUrl\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-azure-table-storage-application-logs-config-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: AzureTableStorageApplicationLogsConfig
---
