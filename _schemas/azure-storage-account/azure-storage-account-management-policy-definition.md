---
description: An object that defines the Lifecycle rule. Each definition is made up with a filters set and an actions set.
layout: schema
name: ManagementPolicyDefinition
properties_list:
- description: An object that defines the action set.
  name: actions
  type: object
- description: An object that defines the filter set.
  name: filters
  type: object
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-management-policy-definition-schema.json
slug: azure-storage-account-management-policy-definition
source_filename: azure-storage-account-management-policy-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-management-policy-definition-schema.json\",\n  \"title\": \"ManagementPolicyDefinition\",\n  \"description\": \"An object that defines the Lifecycle rule. Each definition is made up with a filters set and an actions set.\",\n  \"properties\": {\n    \"actions\": {\n      \"$ref\": \"#/definitions/ManagementPolicyAction\",\n      \"description\": \"An object that defines the action set.\"\n    },\n    \"filters\": {\n      \"$ref\": \"#/definitions/ManagementPolicyFilter\",\n      \"description\": \"An object that defines the filter set.\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"actions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-management-policy-definition-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: ManagementPolicyDefinition
---
