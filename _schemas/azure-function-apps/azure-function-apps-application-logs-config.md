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
tags:
- Azure
- Compute
- FaaS
- Functions
- Serverless
title: ApplicationLogsConfig
---
