---
description: Represents the input of a <code>RetryStageExecution</code> action.
layout: schema
name: RetryStageExecutionInput
properties_list:
- description: ''
  name: pipelineName
  type: object
- description: ''
  name: stageName
  type: object
- description: ''
  name: pipelineExecutionId
  type: object
- description: ''
  name: retryMode
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-retry-stage-execution-input-schema.json
slug: amazon-codepipeline-retry-stage-execution-input
source_filename: amazon-codepipeline-retry-stage-execution-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-retry-stage-execution-input-schema.json\",\n  \"title\": \"RetryStageExecutionInput\",\n  \"description\": \"Represents the input of a <code>RetryStageExecution</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \"The name of the pipeline that contains the failed stage.\"\n        }\n      ]\n    },\n    \"stageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageName\"\n        },\n        {\n          \"description\": \"The name of the failed stage to be retried.\"\n        }\n      ]\n    },\n    \"pipelineExecutionId\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/PipelineExecutionId\"\n        },\n        {\n          \"description\": \"The ID of the pipeline execution in the failed stage to be retried. Use the <a>GetPipelineState</a> action to retrieve the current pipelineExecutionId of the failed stage\"\n        }\n      ]\n    },\n    \"retryMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageRetryMode\"\n        },\n        {\n          \"description\": \"The scope of the retry attempt. Currently, the only supported value is FAILED_ACTIONS.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"pipelineName\",\n    \"stageName\",\n    \"pipelineExecutionId\",\n    \"retryMode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-retry-stage-execution-input-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: RetryStageExecutionInput
---
