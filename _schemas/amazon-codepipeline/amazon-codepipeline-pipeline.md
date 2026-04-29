---
description: Pipeline schema from Amazon CodePipeline
layout: schema
name: Pipeline
properties_list:
- description: The name of the pipeline.
  name: name
  type: string
- description: The ARN of the IAM role used by the pipeline.
  name: roleArn
  type: string
- description: ''
  name: stages
  type: array
- description: The version number of the pipeline.
  name: version
  type: integer
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-pipeline-schema.json
slug: amazon-codepipeline-pipeline
source_filename: amazon-codepipeline-pipeline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-schema.json\",\n  \"title\": \"Pipeline\",\n  \"description\": \"Pipeline schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the pipeline.\"\n    },\n    \"roleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the IAM role used by the pipeline.\"\n    },\n    \"stages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StageDeclaration\"\n      }\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"The version number of the pipeline.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: Pipeline
---
