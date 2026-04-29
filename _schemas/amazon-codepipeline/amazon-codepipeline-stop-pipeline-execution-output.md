---
description: StopPipelineExecutionOutput schema from Amazon CodePipeline
layout: schema
name: StopPipelineExecutionOutput
properties_list:
- description: ''
  name: pipelineExecutionId
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-stop-pipeline-execution-output-schema.json
slug: amazon-codepipeline-stop-pipeline-execution-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-stop-pipeline-execution-output-schema.json\",\n  \"title\": \"StopPipelineExecutionOutput\",\n  \"description\": \"StopPipelineExecutionOutput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineExecutionId\"\n        },\n        {\n          \"description\": \"The unique system-generated ID of the pipeline execution that was stopped.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-stop-pipeline-execution-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: StopPipelineExecutionOutput
---
