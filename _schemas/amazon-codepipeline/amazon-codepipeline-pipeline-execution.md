---
description: PipelineExecution schema from Amazon CodePipeline
layout: schema
name: PipelineExecution
properties_list:
- description: ''
  name: pipelineName
  type: string
- description: ''
  name: pipelineExecutionId
  type: string
- description: ''
  name: pipelineVersion
  type: integer
- description: ''
  name: status
  type: string
- description: ''
  name: statusSummary
  type: string
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-pipeline-execution-schema.json
slug: amazon-codepipeline-pipeline-execution
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-execution-schema.json\",\n  \"title\": \"PipelineExecution\",\n  \"description\": \"PipelineExecution schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineName\": {\n      \"type\": \"string\"\n    },\n    \"pipelineExecutionId\": {\n      \"type\": \"string\"\n    },\n    \"pipelineVersion\": {\n      \"type\": \"integer\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"InProgress\",\n        \"Stopped\",\n        \"Stopping\",\n        \"Succeeded\",\n        \"Superseded\",\n        \"Failed\"\n      ]\n    },\n    \"statusSummary\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-execution-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PipelineExecution
---
