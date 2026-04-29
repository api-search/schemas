---
description: ''
layout: schema
name: RunPipelineRequest
properties_list:
- description: ''
  name: resources
  type: object
- description: ''
  name: variables
  type: object
- description: ''
  name: templateParameters
  type: object
- description: ''
  name: stagesToSkip
  type: array
provider_name: Azure DevOps
provider_slug: azure-devops
schema_file: json-schema/azure-devops-pipelines-run-pipeline-request-schema.json
slug: azure-devops-pipelines-run-pipeline-request
source_filename: azure-devops-pipelines-run-pipeline-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RunPipelineRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resources\": {\n      \"type\": \"object\"\n    },\n    \"variables\": {\n      \"type\": \"object\"\n    },\n    \"templateParameters\": {\n      \"type\": \"object\"\n    },\n    \"stagesToSkip\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/json-schema/azure-devops-pipelines-run-pipeline-request-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Pipelines
- Work Items
title: RunPipelineRequest
---
