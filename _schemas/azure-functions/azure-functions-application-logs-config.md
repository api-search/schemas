---
description: Application logs configuration.
layout: schema
name: ApplicationLogsConfig
properties_list:
- description: Application logs to blob storage configuration.
  name: azureBlobStorage
  type: object
- description: Application logs to azure table storage configuration.
  name: azureTableStorage
  type: object
- description: Application logs to file system configuration.
  name: fileSystem
  type: object
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-application-logs-config-schema.json
slug: azure-functions-application-logs-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-application-logs-config-schema.json\",\n  \"title\": \"ApplicationLogsConfig\",\n  \"description\": \"Application logs configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"azureBlobStorage\": {\n      \"$ref\": \"#/definitions/AzureBlobStorageApplicationLogsConfig\",\n      \"description\": \"Application logs to blob storage configuration.\"\n    },\n    \"azureTableStorage\": {\n      \"$ref\": \"#/definitions/AzureTableStorageApplicationLogsConfig\",\n      \"description\": \"Application logs to azure table storage configuration.\"\n    },\n    \"fileSystem\": {\n      \"$ref\": \"#/definitions/FileSystemApplicationLogsConfig\",\n      \"description\": \"Application logs to file system configuration.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-application-logs-config-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: ApplicationLogsConfig
---
