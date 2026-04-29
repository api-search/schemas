---
description: ''
layout: schema
name: WorkItemRelation
properties_list:
- description: Relation type (e.g., System.LinkTypes.Hierarchy-Forward, System.LinkTypes.Related)
  name: rel
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Azure DevOps
provider_slug: azure-devops
schema_file: json-schema/azure-devops-work-items-work-item-relation-schema.json
slug: azure-devops-work-items-work-item-relation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkItemRelation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rel\": {\n      \"type\": \"string\",\n      \"description\": \"Relation type (e.g., System.LinkTypes.Hierarchy-Forward, System.LinkTypes.Related)\"\n    },\n    \"url\": {\n      \"type\": \"string\"\n    },\n    \"attributes\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/json-schema/azure-devops-work-items-work-item-relation-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Pipelines
- Work Items
title: WorkItemRelation
---
