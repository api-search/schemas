---
description: Represents information about the run of a stage.
layout: schema
name: StageExecution
properties_list:
- description: ''
  name: pipelineExecutionId
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-stage-execution-schema.json
slug: amazon-codepipeline-stage-execution
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-stage-execution-schema.json\",\n  \"title\": \"StageExecution\",\n  \"description\": \"Represents information about the run of a stage.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineExecutionId\"\n        },\n        {\n          \"description\": \"The ID of the pipeline execution associated with the stage.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageExecutionStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the stage, or for a completed stage, the last status of the stage.</p> <note> <p>A status of cancelled means that the pipeline\\u2019s definition\
  \ was updated before the stage execution could be completed.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"pipelineExecutionId\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-stage-execution-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: StageExecution
---
