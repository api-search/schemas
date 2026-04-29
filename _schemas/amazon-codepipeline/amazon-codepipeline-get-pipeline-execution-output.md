---
description: Represents the output of a <code>GetPipelineExecution</code> action.
layout: schema
name: GetPipelineExecutionOutput
properties_list:
- description: ''
  name: pipelineExecution
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-get-pipeline-execution-output-schema.json
slug: amazon-codepipeline-get-pipeline-execution-output
source_filename: amazon-codepipeline-get-pipeline-execution-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-pipeline-execution-output-schema.json\",\n  \"title\": \"GetPipelineExecutionOutput\",\n  \"description\": \"Represents the output of a <code>GetPipelineExecution</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineExecution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineExecution\"\n        },\n        {\n          \"description\": \"Represents information about the execution of a pipeline.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-pipeline-execution-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: GetPipelineExecutionOutput
---
