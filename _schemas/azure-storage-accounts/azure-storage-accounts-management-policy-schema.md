---
description: 'The Storage Account ManagementPolicies Rules. See more details in: https://docs.microsoft.com/en-us/azure/storage/common/storage-lifecycle-managment-concepts.'
layout: schema
name: ManagementPolicySchema
properties_list:
- description: 'The Storage Account ManagementPolicies Rules. See more details in: https://docs.microsoft.com/en-us/azure/storage/common/storage-lifecycle-managment-concepts.'
  name: rules
  type: array
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-management-policy-schema-schema.json
slug: azure-storage-accounts-management-policy-schema
source_filename: azure-storage-accounts-management-policy-schema-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-management-policy-schema-schema.json\",\n  \"title\": \"ManagementPolicySchema\",\n  \"description\": \"The Storage Account ManagementPolicies Rules. See more details in: https://docs.microsoft.com/en-us/azure/storage/common/storage-lifecycle-managment-concepts.\",\n  \"properties\": {\n    \"rules\": {\n      \"description\": \"The Storage Account ManagementPolicies Rules. See more details in: https://docs.microsoft.com/en-us/azure/storage/common/storage-lifecycle-managment-concepts.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ManagementPolicyRule\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"rules\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-management-policy-schema-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ManagementPolicySchema
---
