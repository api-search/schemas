---
description: The blob service properties for blob restore policy
layout: schema
name: RestorePolicyProperties
properties_list:
- description: how long this blob can be restored. It should be great than zero and less than DeleteRetentionPolicy.days.
  name: days
  type: integer
- description: Blob restore is enabled if set to true.
  name: enabled
  type: boolean
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-restore-policy-properties-schema.json
slug: azure-storage-account-restore-policy-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-restore-policy-properties-schema.json\",\n  \"title\": \"RestorePolicyProperties\",\n  \"description\": \"The blob service properties for blob restore policy\",\n  \"properties\": {\n    \"days\": {\n      \"description\": \"how long this blob can be restored. It should be great than zero and less than DeleteRetentionPolicy.days.\",\n      \"maximum\": 365,\n      \"minimum\": 1,\n      \"type\": \"integer\"\n    },\n    \"enabled\": {\n      \"description\": \"Blob restore is enabled if set to true.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"enabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-restore-policy-properties-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: RestorePolicyProperties
---
