---
description: Represents the input of a <code>StartPipelineExecution</code> action.
layout: schema
name: StartPipelineExecutionInput
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: clientRequestToken
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-start-pipeline-execution-input-schema.json
slug: amazon-codepipeline-start-pipeline-execution-input
source_filename: amazon-codepipeline-start-pipeline-execution-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-start-pipeline-execution-input-schema.json\",\n  \"title\": \"StartPipelineExecutionInput\",\n  \"description\": \"Represents the input of a <code>StartPipelineExecution</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \"The name of the pipeline to start.\"\n        }\n      ]\n    },\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"The system-generated unique ID used to identify a unique execution request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-start-pipeline-execution-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: StartPipelineExecutionInput
---
