---
description: An object that wraps the Lifecycle rule. Each rule is uniquely defined by name.
layout: schema
name: ManagementPolicyRule
properties_list:
- description: An object that defines the Lifecycle rule.
  name: definition
  type: object
- description: Rule is enabled if set to true.
  name: enabled
  type: boolean
- description: A rule name can contain any combination of alpha numeric characters. Rule name is case-sensitive. It must be unique within a policy.
  name: name
  type: string
- description: The valid value is Lifecycle
  name: type
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-management-policy-rule-schema.json
slug: azure-storage-accounts-management-policy-rule
source_filename: azure-storage-accounts-management-policy-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-management-policy-rule-schema.json\",\n  \"title\": \"ManagementPolicyRule\",\n  \"description\": \"An object that wraps the Lifecycle rule. Each rule is uniquely defined by name.\",\n  \"properties\": {\n    \"definition\": {\n      \"$ref\": \"#/definitions/ManagementPolicyDefinition\",\n      \"description\": \"An object that defines the Lifecycle rule.\"\n    },\n    \"enabled\": {\n      \"description\": \"Rule is enabled if set to true.\",\n      \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"description\": \"A rule name can contain any combination of alpha numeric characters. Rule name is case-sensitive. It must be unique within a policy.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The valid value is Lifecycle\",\n    \
  \  \"enum\": [\n        \"Lifecycle\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"type\"\n      }\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"type\",\n    \"definition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-management-policy-rule-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ManagementPolicyRule
---
