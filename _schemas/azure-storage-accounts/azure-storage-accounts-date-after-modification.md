---
description: Object to define the number of days after last modification.
layout: schema
name: DateAfterModification
properties_list:
- description: Value indicating the age in days after last modification
  name: daysAfterModificationGreaterThan
  type: number
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-date-after-modification-schema.json
slug: azure-storage-accounts-date-after-modification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-date-after-modification-schema.json\",\n  \"title\": \"DateAfterModification\",\n  \"description\": \"Object to define the number of days after last modification.\",\n  \"properties\": {\n    \"daysAfterModificationGreaterThan\": {\n      \"description\": \"Value indicating the age in days after last modification\",\n      \"minimum\": 0,\n      \"multipleOf\": 1,\n      \"type\": \"number\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"daysAfterModificationGreaterThan\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-date-after-modification-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: DateAfterModification
---
