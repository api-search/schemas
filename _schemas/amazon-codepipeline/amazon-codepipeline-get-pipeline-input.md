---
description: Represents the input of a <code>GetPipeline</code> action.
layout: schema
name: GetPipelineInput
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: version
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-get-pipeline-input-schema.json
slug: amazon-codepipeline-get-pipeline-input
source_filename: amazon-codepipeline-get-pipeline-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-pipeline-input-schema.json\",\n  \"title\": \"GetPipelineInput\",\n  \"description\": \"Represents the input of a <code>GetPipeline</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \"The name of the pipeline for which you want to get information. Pipeline names must be unique in an Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineVersion\"\n        },\n        {\n          \"description\": \"The version number of the pipeline. If you do not specify a version, defaults to the current version.\"\n\
  \        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-pipeline-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: GetPipelineInput
---
