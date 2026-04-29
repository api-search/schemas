---
description: Dimension of blobs, possibly be blob type or access tier.
layout: schema
name: Dimension
properties_list:
- description: Display name of dimension.
  name: displayName
  type: string
- description: Display name of dimension.
  name: name
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-dimension-schema.json
slug: azure-storage-accounts-dimension
source_filename: azure-storage-accounts-dimension-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-dimension-schema.json\",\n  \"title\": \"Dimension\",\n  \"description\": \"Dimension of blobs, possibly be blob type or access tier.\",\n  \"properties\": {\n    \"displayName\": {\n      \"description\": \"Display name of dimension.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Display name of dimension.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-dimension-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: Dimension
---
