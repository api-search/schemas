---
description: CreatePipelineInput schema from Amazon CodePipeline
layout: schema
name: CreatePipelineInput
properties_list:
- description: ''
  name: pipeline
  type: object
- description: ''
  name: tags
  type: array
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-create-pipeline-input-schema.json
slug: amazon-codepipeline-create-pipeline-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-create-pipeline-input-schema.json\",\n  \"title\": \"CreatePipelineInput\",\n  \"description\": \"CreatePipelineInput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipeline\": {\n      \"$ref\": \"#/components/schemas/Pipeline\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    }\n  },\n  \"required\": [\n    \"pipeline\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-create-pipeline-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: CreatePipelineInput
---
