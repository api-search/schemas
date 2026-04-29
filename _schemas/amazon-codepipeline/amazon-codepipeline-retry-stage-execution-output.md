---
description: Represents the output of a <code>RetryStageExecution</code> action.
layout: schema
name: RetryStageExecutionOutput
properties_list:
- description: ''
  name: pipelineExecutionId
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-retry-stage-execution-output-schema.json
slug: amazon-codepipeline-retry-stage-execution-output
source_filename: amazon-codepipeline-retry-stage-execution-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-retry-stage-execution-output-schema.json\",\n  \"title\": \"RetryStageExecutionOutput\",\n  \"description\": \"Represents the output of a <code>RetryStageExecution</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineExecutionId\"\n        },\n        {\n          \"description\": \"The ID of the current workflow execution in the failed stage.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-retry-stage-execution-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: RetryStageExecutionOutput
---
