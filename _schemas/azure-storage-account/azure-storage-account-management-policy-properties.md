---
description: The Storage Account ManagementPolicy properties.
layout: schema
name: ManagementPolicyProperties
properties_list:
- description: Returns the date and time the ManagementPolicies was last modified.
  name: lastModifiedTime
  type: string
- description: 'The Storage Account ManagementPolicy, in JSON format. See more details in: https://docs.microsoft.com/en-us/azure/storage/common/storage-lifecycle-managment-concepts.'
  name: policy
  type: object
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-management-policy-properties-schema.json
slug: azure-storage-account-management-policy-properties
source_filename: azure-storage-account-management-policy-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-management-policy-properties-schema.json\",\n  \"title\": \"ManagementPolicyProperties\",\n  \"description\": \"The Storage Account ManagementPolicy properties.\",\n  \"properties\": {\n    \"lastModifiedTime\": {\n      \"description\": \"Returns the date and time the ManagementPolicies was last modified.\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"policy\": {\n      \"$ref\": \"#/definitions/ManagementPolicySchema\",\n      \"description\": \"The Storage Account ManagementPolicy, in JSON format. See more details in: https://docs.microsoft.com/en-us/azure/storage/common/storage-lifecycle-managment-concepts.\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"policy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-management-policy-properties-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: ManagementPolicyProperties
---
