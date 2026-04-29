---
description: Application logs azure blob storage configuration.
layout: schema
name: AzureBlobStorageApplicationLogsConfig
properties_list:
- description: Log level.
  name: level
  type: string
- description: Retention in days. Remove blobs older than X days. 0 or lower means no retention.
  name: retentionInDays
  type: integer
- description: SAS url to a azure blob container with read/write/list/delete permissions.
  name: sasUrl
  type: string
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-azure-blob-storage-application-logs-config-schema.json
slug: azure-functions-azure-blob-storage-application-logs-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-azure-blob-storage-application-logs-config-schema.json\",\n  \"title\": \"AzureBlobStorageApplicationLogsConfig\",\n  \"description\": \"Application logs azure blob storage configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"level\": {\n      \"description\": \"Log level.\",\n      \"enum\": [\n        \"Off\",\n        \"Verbose\",\n        \"Information\",\n        \"Warning\",\n        \"Error\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"LogLevel\"\n      }\n    },\n    \"retentionInDays\": {\n      \"description\": \"Retention in days.\\nRemove blobs older than X days.\\n0 or lower means no retention.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"sasUrl\": {\n\
  \      \"description\": \"SAS url to a azure blob container with read/write/list/delete permissions.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-azure-blob-storage-application-logs-config-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: AzureBlobStorageApplicationLogsConfig
---
