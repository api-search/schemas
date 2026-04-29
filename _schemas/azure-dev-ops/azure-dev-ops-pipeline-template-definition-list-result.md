---
description: Result of a request to list all pipeline template definitions.
layout: schema
name: PipelineTemplateDefinitionListResult
properties_list:
- description: The URL to get the next set of pipeline template definitions, if there are any.
  name: nextLink
  type: string
- description: List of pipeline template definitions.
  name: value
  type: array
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-pipeline-template-definition-list-result-schema.json
slug: azure-dev-ops-pipeline-template-definition-list-result
source_filename: azure-dev-ops-pipeline-template-definition-list-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-pipeline-template-definition-list-result-schema.json\",\n  \"title\": \"PipelineTemplateDefinitionListResult\",\n  \"description\": \"Result of a request to list all pipeline template definitions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"The URL to get the next set of pipeline template definitions, if there are any.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"List of pipeline template definitions.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/PipelineTemplateDefinition\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-pipeline-template-definition-list-result-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: PipelineTemplateDefinitionListResult
---
