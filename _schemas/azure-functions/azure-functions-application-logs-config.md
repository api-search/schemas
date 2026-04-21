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
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: ApplicationLogsConfig
---
