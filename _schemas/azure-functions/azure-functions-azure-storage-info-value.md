---
description: Azure Files or Blob Storage access information value for dictionary storage.
layout: schema
name: AzureStorageInfoValue
properties_list:
- description: Access key for the storage account.
  name: accessKey
  type: string
- description: Name of the storage account.
  name: accountName
  type: string
- description: Path to mount the storage within the site's runtime environment.
  name: mountPath
  type: string
- description: Name of the file share (container name, for Blob storage).
  name: shareName
  type: string
- description: State of the storage account.
  name: state
  type: string
- description: Type of storage.
  name: type
  type: string
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-azure-storage-info-value-schema.json
slug: azure-functions-azure-storage-info-value
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: AzureStorageInfoValue
---
