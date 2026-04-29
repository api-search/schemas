---
description: ''
layout: schema
name: PipelineRun
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: result
  type: string
- description: ''
  name: createdDate
  type: string
- description: ''
  name: finishedDate
  type: string
- description: ''
  name: pipeline
  type: object
- description: ''
  name: resources
  type: object
- description: ''
  name: variables
  type: object
- description: ''
  name: url
  type: string
provider_name: Azure DevOps
provider_slug: azure-devops
schema_file: json-schema/azure-devops-pipelines-pipeline-run-schema.json
slug: azure-devops-pipelines-pipeline-run
source_filename: azure-devops-pipelines-pipeline-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PipelineRun\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"result\": {\n      \"type\": \"string\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\"\n    },\n    \"finishedDate\": {\n      \"type\": \"string\"\n    },\n    \"pipeline\": {\n      \"type\": \"object\"\n    },\n    \"resources\": {\n      \"type\": \"object\"\n    },\n    \"variables\": {\n      \"type\": \"object\"\n    },\n    \"url\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/json-schema/azure-devops-pipelines-pipeline-run-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Pipelines
- Work Items
title: PipelineRun
---
