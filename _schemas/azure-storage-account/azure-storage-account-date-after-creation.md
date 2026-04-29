---
description: Object to define the number of days after creation.
layout: schema
name: DateAfterCreation
properties_list:
- description: Value indicating the age in days after creation
  name: daysAfterCreationGreaterThan
  type: number
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-date-after-creation-schema.json
slug: azure-storage-account-date-after-creation
source_filename: azure-storage-account-date-after-creation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-date-after-creation-schema.json\",\n  \"title\": \"DateAfterCreation\",\n  \"description\": \"Object to define the number of days after creation.\",\n  \"properties\": {\n    \"daysAfterCreationGreaterThan\": {\n      \"description\": \"Value indicating the age in days after creation\",\n      \"minimum\": 0,\n      \"multipleOf\": 1,\n      \"type\": \"number\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"daysAfterCreationGreaterThan\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-date-after-creation-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: DateAfterCreation
---
