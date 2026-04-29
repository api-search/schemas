---
description: ''
layout: schema
name: Error
properties_list:
- description: ''
  name: message
  type: string
- description: ''
  name: errorCode
  type: integer
provider_name: Azure DevOps
provider_slug: azure-devops
schema_file: json-schema/azure-devops-pipelines-error-schema.json
slug: azure-devops-pipelines-error
source_filename: azure-devops-pipelines-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"errorCode\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/json-schema/azure-devops-pipelines-error-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Pipelines
- Work Items
title: Error
---
