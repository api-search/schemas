---
description: The interaction that stopped a pipeline execution.
layout: schema
name: StopExecutionTrigger
properties_list:
- description: ''
  name: reason
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-stop-execution-trigger-schema.json
slug: amazon-codepipeline-stop-execution-trigger
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-stop-execution-trigger-schema.json\",\n  \"title\": \"StopExecutionTrigger\",\n  \"description\": \"The interaction that stopped a pipeline execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StopPipelineExecutionReason\"\n        },\n        {\n          \"description\": \"The user-specified reason the pipeline was stopped.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-stop-execution-trigger-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: StopExecutionTrigger
---
