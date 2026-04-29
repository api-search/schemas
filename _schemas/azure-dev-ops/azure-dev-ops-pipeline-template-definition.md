---
description: Definition of a pipeline template.
layout: schema
name: PipelineTemplateDefinition
properties_list:
- description: Description of the pipeline enabled by the template.
  name: description
  type: string
- description: Unique identifier of the pipeline template.
  name: id
  type: string
- description: List of input parameters required by the template to create a pipeline.
  name: inputs
  type: array
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-pipeline-template-definition-schema.json
slug: azure-dev-ops-pipeline-template-definition
source_filename: azure-dev-ops-pipeline-template-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-pipeline-template-definition-schema.json\",\n  \"title\": \"PipelineTemplateDefinition\",\n  \"description\": \"Definition of a pipeline template.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"Description of the pipeline enabled by the template.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"Unique identifier of the pipeline template.\",\n      \"type\": \"string\"\n    },\n    \"inputs\": {\n      \"description\": \"List of input parameters required by the template to create a pipeline.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/InputDescriptor\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-pipeline-template-definition-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: PipelineTemplateDefinition
---
