---
description: Represents the output of a <code>StartPipelineExecution</code> action.
layout: schema
name: StartPipelineExecutionOutput
properties_list:
- description: ''
  name: pipelineExecutionId
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-start-pipeline-execution-output-schema.json
slug: amazon-codepipeline-start-pipeline-execution-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-start-pipeline-execution-output-schema.json\",\n  \"title\": \"StartPipelineExecutionOutput\",\n  \"description\": \"Represents the output of a <code>StartPipelineExecution</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineExecutionId\"\n        },\n        {\n          \"description\": \"The unique system-generated ID of the pipeline execution that was started.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-start-pipeline-execution-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: StartPipelineExecutionOutput
---
