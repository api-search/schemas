---
description: Blob restore parameters
layout: schema
name: BlobRestoreParameters
properties_list:
- description: Blob ranges to restore.
  name: blobRanges
  type: array
- description: Restore blob to the specified time.
  name: timeToRestore
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-blob-restore-parameters-schema.json
slug: azure-storage-accounts-blob-restore-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-blob-restore-parameters-schema.json\",\n  \"title\": \"BlobRestoreParameters\",\n  \"description\": \"Blob restore parameters\",\n  \"properties\": {\n    \"blobRanges\": {\n      \"description\": \"Blob ranges to restore.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/BlobRestoreRange\"\n      },\n      \"type\": \"array\"\n    },\n    \"timeToRestore\": {\n      \"description\": \"Restore blob to the specified time.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"timeToRestore\",\n    \"blobRanges\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-blob-restore-parameters-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: BlobRestoreParameters
---
