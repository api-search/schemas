---
description: Represents the input of a <code>DeletePipeline</code> action.
layout: schema
name: DeletePipelineInput
properties_list:
- description: ''
  name: name
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-delete-pipeline-input-schema.json
slug: amazon-codepipeline-delete-pipeline-input
source_filename: amazon-codepipeline-delete-pipeline-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-delete-pipeline-input-schema.json\",\n  \"title\": \"DeletePipelineInput\",\n  \"description\": \"Represents the input of a <code>DeletePipeline</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \"The name of the pipeline to be deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-delete-pipeline-input-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: DeletePipelineInput
---
