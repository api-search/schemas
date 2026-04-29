---
description: ''
layout: schema
name: WorkItemField
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: referenceName
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: readOnly
  type: boolean
- description: ''
  name: isQueryable
  type: boolean
- description: ''
  name: isIdentity
  type: boolean
provider_name: Azure DevOps
provider_slug: azure-devops
schema_file: json-schema/azure-devops-work-items-work-item-field-schema.json
slug: azure-devops-work-items-work-item-field
source_filename: azure-devops-work-items-work-item-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkItemField\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"referenceName\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"readOnly\": {\n      \"type\": \"boolean\"\n    },\n    \"isQueryable\": {\n      \"type\": \"boolean\"\n    },\n    \"isIdentity\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/json-schema/azure-devops-work-items-work-item-field-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Pipelines
- Work Items
title: WorkItemField
---
