---
description: Request body for creating a function URL
layout: schema
name: CreateFunctionUrlConfigRequest
properties_list:
- description: The type of authentication. NONE allows public unauthenticated access. AWS_IAM requires IAM authentication.
  name: AuthType
  type: string
- description: ''
  name: InvokeMode
  type: string
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-create-function-url-config-request-schema.json
slug: aws-lambda-create-function-url-config-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateFunctionUrlConfigRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a function URL\",\n  \"properties\": {\n    \"AuthType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of authentication. NONE allows public unauthenticated access. AWS_IAM requires IAM authentication.\"\n    },\n    \"InvokeMode\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-create-function-url-config-request-schema.json
tags: []
title: CreateFunctionUrlConfigRequest
---
