---
description: ''
layout: schema
name: CreatePipelineRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: folder
  type: string
- description: ''
  name: configuration
  type: object
provider_name: Azure DevOps
provider_slug: azure-devops
schema_file: json-schema/azure-devops-pipelines-create-pipeline-request-schema.json
slug: azure-devops-pipelines-create-pipeline-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreatePipelineRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"folder\": {\n      \"type\": \"string\"\n    },\n    \"configuration\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/json-schema/azure-devops-pipelines-create-pipeline-request-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Pipelines
- Work Items
title: CreatePipelineRequest
---
