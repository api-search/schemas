---
description: BlobServiceItems schema from Azure Storage Accounts API
layout: schema
name: BlobServiceItems
properties_list:
- description: List of blob services returned.
  name: value
  type: array
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-blob-service-items-schema.json
slug: azure-storage-accounts-blob-service-items
source_filename: azure-storage-accounts-blob-service-items-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-blob-service-items-schema.json\",\n  \"title\": \"BlobServiceItems\",\n  \"description\": \"BlobServiceItems schema from Azure Storage Accounts API\",\n  \"properties\": {\n    \"value\": {\n      \"description\": \"List of blob services returned.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/BlobServiceProperties\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-blob-service-items-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: BlobServiceItems
---
