---
description: Azure DevOps work item
layout: schema
name: WorkItem
properties_list:
- description: Work item ID
  name: id
  type: integer
- description: Revision number
  name: rev
  type: integer
- description: Work item field values
  name: fields
  type: object
- description: ''
  name: relations
  type: array
- description: ''
  name: url
  type: string
provider_name: Azure DevOps
provider_slug: azure-devops
schema_file: json-schema/azure-devops-work-items-work-item-schema.json
slug: azure-devops-work-items-work-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkItem\",\n  \"type\": \"object\",\n  \"description\": \"Azure DevOps work item\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Work item ID\"\n    },\n    \"rev\": {\n      \"type\": \"integer\",\n      \"description\": \"Revision number\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"Work item field values\"\n    },\n    \"relations\": {\n      \"type\": \"array\"\n    },\n    \"url\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/json-schema/azure-devops-work-items-work-item-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Pipelines
- Work Items
title: WorkItem
---
