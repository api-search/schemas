---
description: ''
layout: schema
name: WiqlResult
properties_list:
- description: ''
  name: queryType
  type: string
- description: ''
  name: asOf
  type: string
- description: ''
  name: workItems
  type: array
- description: ''
  name: workItemRelations
  type: array
provider_name: Azure DevOps
provider_slug: azure-devops
schema_file: json-schema/azure-devops-work-items-wiql-result-schema.json
slug: azure-devops-work-items-wiql-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WiqlResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queryType\": {\n      \"type\": \"string\"\n    },\n    \"asOf\": {\n      \"type\": \"string\"\n    },\n    \"workItems\": {\n      \"type\": \"array\"\n    },\n    \"workItemRelations\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/json-schema/azure-devops-work-items-wiql-result-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Pipelines
- Work Items
title: WiqlResult
---
