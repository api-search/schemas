---
description: Request body for updating a function URL configuration
layout: schema
name: UpdateFunctionUrlConfigRequest
properties_list:
- description: ''
  name: AuthType
  type: string
- description: ''
  name: InvokeMode
  type: string
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-update-function-url-config-request-schema.json
slug: aws-lambda-update-function-url-config-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateFunctionUrlConfigRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a function URL configuration\",\n  \"properties\": {\n    \"AuthType\": {\n      \"type\": \"string\"\n    },\n    \"InvokeMode\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-update-function-url-config-request-schema.json
tags: []
title: UpdateFunctionUrlConfigRequest
---
