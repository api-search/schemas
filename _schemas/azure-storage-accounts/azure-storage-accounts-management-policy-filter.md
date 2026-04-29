---
description: Filters limit rule actions to a subset of blobs within the storage account. If multiple filters are defined, a logical AND is performed on all filters.
layout: schema
name: ManagementPolicyFilter
properties_list:
- description: An array of predefined enum values. Only blockBlob is supported.
  name: blobTypes
  type: array
- description: An array of strings for prefixes to be match.
  name: prefixMatch
  type: array
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-management-policy-filter-schema.json
slug: azure-storage-accounts-management-policy-filter
source_filename: azure-storage-accounts-management-policy-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-management-policy-filter-schema.json\",\n  \"title\": \"ManagementPolicyFilter\",\n  \"description\": \"Filters limit rule actions to a subset of blobs within the storage account. If multiple filters are defined, a logical AND is performed on all filters. \",\n  \"properties\": {\n    \"blobTypes\": {\n      \"description\": \"An array of predefined enum values. Only blockBlob is supported.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"prefixMatch\": {\n      \"description\": \"An array of strings for prefixes to be match.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"blobTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-management-policy-filter-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ManagementPolicyFilter
---
