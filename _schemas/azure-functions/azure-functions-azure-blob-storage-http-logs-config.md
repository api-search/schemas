---
description: Http logs to azure blob storage configuration.
layout: schema
name: AzureBlobStorageHttpLogsConfig
properties_list:
- description: True if configuration is enabled, false if it is disabled and null if configuration is not set.
  name: enabled
  type: boolean
- description: Retention in days. Remove blobs older than X days. 0 or lower means no retention.
  name: retentionInDays
  type: integer
- description: SAS url to a azure blob container with read/write/list/delete permissions.
  name: sasUrl
  type: string
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-azure-blob-storage-http-logs-config-schema.json
slug: azure-functions-azure-blob-storage-http-logs-config
source_filename: azure-functions-azure-blob-storage-http-logs-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-azure-blob-storage-http-logs-config-schema.json\",\n  \"title\": \"AzureBlobStorageHttpLogsConfig\",\n  \"description\": \"Http logs to azure blob storage configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"description\": \"True if configuration is enabled, false if it is disabled and null if configuration is not set.\",\n      \"type\": \"boolean\"\n    },\n    \"retentionInDays\": {\n      \"description\": \"Retention in days.\\nRemove blobs older than X days.\\n0 or lower means no retention.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"sasUrl\": {\n      \"description\": \"SAS url to a azure blob container with read/write/list/delete permissions.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-azure-blob-storage-http-logs-config-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: AzureBlobStorageHttpLogsConfig
---
