---
description: Display information of an operation.
layout: schema
name: OperationDisplayValue
properties_list:
- description: Friendly description of the operation.
  name: description
  type: string
- description: Friendly name of the operation.
  name: operation
  type: string
- description: Friendly name of the resource provider.
  name: provider
  type: string
- description: Friendly name of the resource type the operation applies to.
  name: resource
  type: string
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-operation-display-value-schema.json
slug: azure-dev-ops-operation-display-value
source_filename: azure-dev-ops-operation-display-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-operation-display-value-schema.json\",\n  \"title\": \"OperationDisplayValue\",\n  \"description\": \"Display information of an operation.\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"Friendly description of the operation.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"operation\": {\n      \"description\": \"Friendly name of the operation.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"provider\": {\n      \"description\": \"Friendly name of the resource provider.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"resource\": {\n      \"description\": \"Friendly name of the resource type the operation applies to.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  },\n  \"\
  type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-operation-display-value-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: OperationDisplayValue
---
