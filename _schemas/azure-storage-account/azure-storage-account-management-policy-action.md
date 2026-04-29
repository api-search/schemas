---
description: Actions are applied to the filtered blobs when the execution condition is met.
layout: schema
name: ManagementPolicyAction
properties_list:
- description: The management policy action for base blob
  name: baseBlob
  type: object
- description: The management policy action for snapshot
  name: snapshot
  type: object
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-management-policy-action-schema.json
slug: azure-storage-account-management-policy-action
source_filename: azure-storage-account-management-policy-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-management-policy-action-schema.json\",\n  \"title\": \"ManagementPolicyAction\",\n  \"description\": \"Actions are applied to the filtered blobs when the execution condition is met.\",\n  \"properties\": {\n    \"baseBlob\": {\n      \"$ref\": \"#/definitions/ManagementPolicyBaseBlob\",\n      \"description\": \"The management policy action for base blob\"\n    },\n    \"snapshot\": {\n      \"$ref\": \"#/definitions/ManagementPolicySnapShot\",\n      \"description\": \"The management policy action for snapshot\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-management-policy-action-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: ManagementPolicyAction
---
