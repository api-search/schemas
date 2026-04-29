---
description: The Get Storage Account ManagementPolicies operation response.
layout: schema
name: ManagementPolicy
properties_list:
- description: Returns the Storage Account Data Policies Rules.
  name: properties
  type: object
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-management-policy-schema.json
slug: azure-storage-account-management-policy
source_filename: azure-storage-account-management-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-management-policy-schema.json\",\n  \"title\": \"ManagementPolicy\",\n  \"description\": \"The Get Storage Account ManagementPolicies operation response.\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/ManagementPolicyProperties\",\n      \"description\": \"Returns the Storage Account Data Policies Rules.\",\n      \"x-ms-client-flatten\": true\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-management-policy-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: ManagementPolicy
---
