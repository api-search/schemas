---
description: Configuration for a Lambda function URL
layout: schema
name: FunctionUrlConfig
properties_list:
- description: The HTTP URL endpoint for the function
  name: FunctionUrl
  type: string
- description: The ARN of the function
  name: FunctionArn
  type: string
- description: The type of authentication the function URL uses
  name: AuthType
  type: string
- description: When the function URL was created in ISO 8601 format
  name: CreationTime
  type: string
- description: When the function URL was last modified
  name: LastModifiedTime
  type: string
- description: Use BUFFERED for synchronous invocation or RESPONSE_STREAM for response streaming
  name: InvokeMode
  type: string
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-function-url-config-schema.json
slug: aws-lambda-function-url-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FunctionUrlConfig\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for a Lambda function URL\",\n  \"properties\": {\n    \"FunctionUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP URL endpoint for the function\"\n    },\n    \"FunctionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the function\"\n    },\n    \"AuthType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of authentication the function URL uses\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"description\": \"When the function URL was created in ISO 8601 format\"\n    },\n    \"LastModifiedTime\": {\n      \"type\": \"string\",\n      \"description\": \"When the function URL was last modified\"\n    },\n    \"InvokeMode\": {\n      \"type\": \"string\",\n      \"description\": \"Use BUFFERED for synchronous invocation or\
  \ RESPONSE_STREAM for response streaming\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-function-url-config-schema.json
tags: []
title: FunctionUrlConfig
---
