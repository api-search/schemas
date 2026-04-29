---
description: ''
layout: schema
name: JsonPatchOperation
properties_list:
- description: ''
  name: op
  type: string
- description: JSON Pointer path to the field
  name: path
  type: string
- description: New value for add/replace operations
  name: value
  type: string
- description: Source path for copy/move operations
  name: from
  type: string
provider_name: Azure DevOps
provider_slug: azure-devops
schema_file: json-schema/azure-devops-work-items-json-patch-operation-schema.json
slug: azure-devops-work-items-json-patch-operation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JsonPatchOperation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"op\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"JSON Pointer path to the field\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"New value for add/replace operations\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"Source path for copy/move operations\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/json-schema/azure-devops-work-items-json-patch-operation-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Pipelines
- Work Items
title: JsonPatchOperation
---
