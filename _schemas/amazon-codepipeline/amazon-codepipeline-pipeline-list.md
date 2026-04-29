---
description: PipelineList schema from Amazon CodePipeline
layout: schema
name: PipelineList
properties_list:
- description: ''
  name: pipelines
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-pipeline-list-schema.json
slug: amazon-codepipeline-pipeline-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-list-schema.json\",\n  \"title\": \"PipelineList\",\n  \"description\": \"PipelineList schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelines\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"version\": {\n            \"type\": \"integer\"\n          },\n          \"created\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"updated\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-list-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PipelineList
---
