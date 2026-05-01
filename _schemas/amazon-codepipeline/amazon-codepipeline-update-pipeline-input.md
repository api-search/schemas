---
description: Represents the input of an <code>UpdatePipeline</code> action.
layout: schema
name: UpdatePipelineInput
properties_list:
- description: ''
  name: pipeline
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-update-pipeline-input-schema.json
slug: amazon-codepipeline-update-pipeline-input
source_filename: amazon-codepipeline-update-pipeline-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-update-pipeline-input-schema.json\",\n  \"title\": \"UpdatePipelineInput\",\n  \"description\": \"Represents the input of an <code>UpdatePipeline</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipeline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineDeclaration\"\n        },\n        {\n          \"description\": \"The name of the pipeline to be updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"pipeline\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-update-pipeline-input-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: UpdatePipelineInput
---
