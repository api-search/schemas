---
description: Blob range
layout: schema
name: BlobRestoreRange
properties_list:
- description: Blob end range. Empty means account end.
  name: endRange
  type: string
- description: Blob start range. Empty means account start.
  name: startRange
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-blob-restore-range-schema.json
slug: azure-storage-accounts-blob-restore-range
source_filename: azure-storage-accounts-blob-restore-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-blob-restore-range-schema.json\",\n  \"title\": \"BlobRestoreRange\",\n  \"description\": \"Blob range\",\n  \"properties\": {\n    \"endRange\": {\n      \"description\": \"Blob end range. Empty means account end.\",\n      \"type\": \"string\"\n    },\n    \"startRange\": {\n      \"description\": \"Blob start range. Empty means account start.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"startRange\",\n    \"endRange\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-blob-restore-range-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: BlobRestoreRange
---
