---
description: LambdaFunctionArn schema from Amazon CodePipeline
layout: schema
name: LambdaFunctionArn
properties_list: []
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-lambda-function-arn-schema.json
slug: amazon-codepipeline-lambda-function-arn
source_filename: amazon-codepipeline-lambda-function-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-lambda-function-arn-schema.json\",\n  \"title\": \"LambdaFunctionArn\",\n  \"description\": \"LambdaFunctionArn schema from Amazon CodePipeline\",\n  \"type\": \"string\",\n  \"pattern\": \"arn:aws(-[\\\\w]+)*:lambda:.+:[0-9]{12}:function:.+\",\n  \"minLength\": 1,\n  \"maxLength\": 140\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-lambda-function-arn-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: LambdaFunctionArn
---
