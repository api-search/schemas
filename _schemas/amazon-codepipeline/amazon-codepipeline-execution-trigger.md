---
description: The interaction or event that started a pipeline execution.
layout: schema
name: ExecutionTrigger
properties_list:
- description: ''
  name: triggerType
  type: object
- description: ''
  name: triggerDetail
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-execution-trigger-schema.json
slug: amazon-codepipeline-execution-trigger
source_filename: amazon-codepipeline-execution-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-execution-trigger-schema.json\",\n  \"title\": \"ExecutionTrigger\",\n  \"description\": \"The interaction or event that started a pipeline execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"triggerType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerType\"\n        },\n        {\n          \"description\": \"The type of change-detection method, command, or user interaction that started a pipeline execution.\"\n        }\n      ]\n    },\n    \"triggerDetail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerDetail\"\n        },\n        {\n          \"description\": \"Detail related to the event that started a pipeline execution, such as the webhook ARN of the webhook that triggered the pipeline\
  \ execution or the user ARN for a user-initiated <code>start-pipeline-execution</code> CLI command.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-execution-trigger-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ExecutionTrigger
---
