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
provider_name: Azure Function Apps
provider_slug: azure-function-apps
schema_file: json-schema/azure-function-apps-azure-storage-info-value-schema.json
slug: azure-function-apps-azure-storage-info-value
tags:
- Azure
- Compute
- FaaS
- Functions
- Serverless
title: AzureStorageInfoValue
---
