---
description: Template used to bootstrap the pipeline.
layout: schema
name: PipelineTemplate
properties_list:
- description: Unique identifier of the pipeline template.
  name: id
  type: string
- description: Dictionary of input parameters used in the pipeline template.
  name: parameters
  type: object
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-pipeline-template-schema.json
slug: azure-dev-ops-pipeline-template
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-pipeline-template-schema.json\",\n  \"title\": \"PipelineTemplate\",\n  \"description\": \"Template used to bootstrap the pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Unique identifier of the pipeline template.\",\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Dictionary of input parameters used in the pipeline template.\",\n      \"type\": \"object\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-pipeline-template-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: PipelineTemplate
---
