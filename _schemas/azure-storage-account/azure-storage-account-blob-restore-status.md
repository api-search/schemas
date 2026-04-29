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
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-blob-restore-status-schema.json
slug: azure-storage-account-blob-restore-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-blob-restore-status-schema.json\",\n  \"title\": \"BlobRestoreStatus\",\n  \"description\": \"Blob restore status.\",\n  \"properties\": {\n    \"failureReason\": {\n      \"description\": \"Failure reason when blob restore is failed.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"$ref\": \"#/definitions/BlobRestoreParameters\",\n      \"description\": \"Blob restore request parameters.\",\n      \"readOnly\": true\n    },\n    \"restoreId\": {\n      \"description\": \"Id for tracking blob restore request.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of blob restore progress. Possible values are: - InProgress: Indicates that blob restore is ongoing.\
  \ - Complete: Indicates that blob restore has been completed successfully. - Failed: Indicates that blob restore is failed.\",\n      \"enum\": [\n        \"InProgress\",\n        \"Complete\",\n        \"Failed\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"BlobRestoreProgressStatus\"\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-blob-restore-status-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: BlobRestoreStatus
---
