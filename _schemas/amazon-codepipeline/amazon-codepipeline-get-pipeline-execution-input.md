---
description: Represents the input of a <code>GetPipelineExecution</code> action.
layout: schema
name: GetPipelineExecutionInput
properties_list:
- description: ''
  name: pipelineName
  type: object
- description: ''
  name: pipelineExecutionId
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-get-pipeline-execution-input-schema.json
slug: amazon-codepipeline-get-pipeline-execution-input
source_filename: amazon-codepipeline-get-pipeline-execution-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-pipeline-execution-input-schema.json\",\n  \"title\": \"GetPipelineExecutionInput\",\n  \"description\": \"Represents the input of a <code>GetPipelineExecution</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \"The name of the pipeline about which you want to get execution details.\"\n        }\n      ]\n    },\n    \"pipelineExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineExecutionId\"\n        },\n        {\n          \"description\": \"The ID of the pipeline execution about which you want to get execution details.\"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"pipelineName\",\n    \"pipelineExecutionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-pipeline-execution-input-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: GetPipelineExecutionInput
---
