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
provider_name: Azure Function Apps
provider_slug: azure-function-apps
schema_file: json-schema/azure-function-apps-application-logs-config-schema.json
slug: azure-function-apps-application-logs-config
source_filename: azure-function-apps-application-logs-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-application-logs-config-schema.json\",\n  \"title\": \"ApplicationLogsConfig\",\n  \"description\": \"Application logs configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"azureBlobStorage\": {\n      \"$ref\": \"#/definitions/AzureBlobStorageApplicationLogsConfig\",\n      \"description\": \"Application logs to blob storage configuration.\"\n    },\n    \"azureTableStorage\": {\n      \"$ref\": \"#/definitions/AzureTableStorageApplicationLogsConfig\",\n      \"description\": \"Application logs to azure table storage configuration.\"\n    },\n    \"fileSystem\": {\n      \"$ref\": \"#/definitions/FileSystemApplicationLogsConfig\",\n      \"description\": \"Application logs to file system configuration.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-application-logs-config-schema.json
tags:
- Azure
- Compute
- FaaS
- Functions
- Serverless
title: ApplicationLogsConfig
---
