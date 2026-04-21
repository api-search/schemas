---
description: Blob restore status.
layout: schema
name: BlobRestoreStatus
properties_list:
- description: Failure reason when blob restore is failed.
  name: failureReason
  type: string
- description: Blob restore request parameters.
  name: parameters
  type: object
- description: Id for tracking blob restore request.
  name: restoreId
  type: string
- description: 'The status of blob restore progress. Possible values are: - InProgress: Indicates that blob restore is ongoing. - Complete: Indicates that blob restore has been completed successfully. - Failed: Indic'
  name: status
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-blob-restore-status-schema.json
slug: azure-storage-accounts-blob-restore-status
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: BlobRestoreStatus
---
