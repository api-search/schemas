---
description: The blob service properties for change feed events.
layout: schema
name: ChangeFeed
properties_list:
- description: Indicates whether change feed event logging is enabled for the Blob service.
  name: enabled
  type: boolean
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-change-feed-schema.json
slug: azure-storage-accounts-change-feed
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-change-feed-schema.json\",\n  \"title\": \"ChangeFeed\",\n  \"description\": \"The blob service properties for change feed events.\",\n  \"properties\": {\n    \"enabled\": {\n      \"description\": \"Indicates whether change feed event logging is enabled for the Blob service.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-change-feed-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ChangeFeed
---
