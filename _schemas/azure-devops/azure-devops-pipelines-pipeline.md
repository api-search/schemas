---
description: ''
layout: schema
name: Pipeline
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: revision
  type: integer
- description: ''
  name: folder
  type: string
- description: ''
  name: configuration
  type: object
- description: ''
  name: url
  type: string
- description: ''
  name: links
  type: object
provider_name: Azure DevOps
provider_slug: azure-devops
schema_file: json-schema/azure-devops-pipelines-pipeline-schema.json
slug: azure-devops-pipelines-pipeline
source_filename: azure-devops-pipelines-pipeline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Pipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"revision\": {\n      \"type\": \"integer\"\n    },\n    \"folder\": {\n      \"type\": \"string\"\n    },\n    \"configuration\": {\n      \"type\": \"object\"\n    },\n    \"url\": {\n      \"type\": \"string\"\n    },\n    \"links\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/json-schema/azure-devops-pipelines-pipeline-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Pipelines
- Work Items
title: Pipeline
---
