---
description: Result of a request to list all Azure Pipelines under a given scope.
layout: schema
name: PipelineListResult
properties_list:
- description: URL to get the next set of Pipelines, if there are any.
  name: nextLink
  type: string
- description: List of pipelines.
  name: value
  type: array
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-pipeline-list-result-schema.json
slug: azure-dev-ops-pipeline-list-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-pipeline-list-result-schema.json\",\n  \"title\": \"PipelineListResult\",\n  \"description\": \"Result of a request to list all Azure Pipelines under a given scope.\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"URL to get the next set of Pipelines, if there are any.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"List of pipelines.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Pipeline\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-pipeline-list-result-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: PipelineListResult
---
