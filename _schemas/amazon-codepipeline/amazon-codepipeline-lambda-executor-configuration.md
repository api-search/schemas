---
description: Details about the configuration for the <code>Lambda</code> action engine, or executor.
layout: schema
name: LambdaExecutorConfiguration
properties_list:
- description: ''
  name: lambdaFunctionArn
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-lambda-executor-configuration-schema.json
slug: amazon-codepipeline-lambda-executor-configuration
source_filename: amazon-codepipeline-lambda-executor-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-lambda-executor-configuration-schema.json\",\n  \"title\": \"LambdaExecutorConfiguration\",\n  \"description\": \"Details about the configuration for the <code>Lambda</code> action engine, or executor.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lambdaFunctionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionArn\"\n        },\n        {\n          \"description\": \"The ARN of the Lambda function used by the action engine.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"lambdaFunctionArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-lambda-executor-configuration-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: LambdaExecutorConfiguration
---
