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
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: AzureTableStorageApplicationLogsConfig
---
