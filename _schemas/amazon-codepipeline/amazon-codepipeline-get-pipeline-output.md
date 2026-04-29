---
description: Represents the output of a <code>GetPipeline</code> action.
layout: schema
name: GetPipelineOutput
properties_list:
- description: ''
  name: pipeline
  type: object
- description: ''
  name: metadata
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-get-pipeline-output-schema.json
slug: amazon-codepipeline-get-pipeline-output
source_filename: amazon-codepipeline-get-pipeline-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-pipeline-output-schema.json\",\n  \"title\": \"GetPipelineOutput\",\n  \"description\": \"Represents the output of a <code>GetPipeline</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipeline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineDeclaration\"\n        },\n        {\n          \"description\": \"Represents the structure of actions and stages to be performed in the pipeline. \"\n        }\n      ]\n    },\n    \"metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineMetadata\"\n        },\n        {\n          \"description\": \"Represents the pipeline metadata information returned as part of the output of a <code>GetPipeline</code> action.\"\n        }\n      ]\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-pipeline-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: GetPipelineOutput
---
