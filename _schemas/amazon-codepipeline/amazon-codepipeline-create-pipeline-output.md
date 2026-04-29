---
description: Represents the output of a <code>CreatePipeline</code> action.
layout: schema
name: CreatePipelineOutput
properties_list:
- description: ''
  name: pipeline
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-create-pipeline-output-schema.json
slug: amazon-codepipeline-create-pipeline-output
source_filename: amazon-codepipeline-create-pipeline-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-create-pipeline-output-schema.json\",\n  \"title\": \"CreatePipelineOutput\",\n  \"description\": \"Represents the output of a <code>CreatePipeline</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipeline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineDeclaration\"\n        },\n        {\n          \"description\": \"Represents the structure of actions and stages to be performed in the pipeline. \"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"Specifies the tags applied to the pipeline.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-create-pipeline-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: CreatePipelineOutput
---
