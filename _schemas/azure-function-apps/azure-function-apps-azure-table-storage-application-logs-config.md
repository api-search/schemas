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
provider_name: Azure Function Apps
provider_slug: azure-function-apps
schema_file: json-schema/azure-function-apps-azure-table-storage-application-logs-config-schema.json
slug: azure-function-apps-azure-table-storage-application-logs-config
tags:
- Azure
- Compute
- FaaS
- Functions
- Serverless
title: AzureTableStorageApplicationLogsConfig
---
