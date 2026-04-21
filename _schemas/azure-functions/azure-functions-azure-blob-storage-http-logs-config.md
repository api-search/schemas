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
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: AzureBlobStorageHttpLogsConfig
---
