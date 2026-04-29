---
description: Error response from the Lambda API
layout: schema
name: ErrorResponse
properties_list:
- description: The error type
  name: Type
  type: string
- description: The error message
  name: Message
  type: string
- description: The error code
  name: Code
  type: string
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-error-response-schema.json
slug: aws-lambda-error-response
source_filename: aws-lambda-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Error response from the Lambda API\",\n  \"properties\": {\n    \"Type\": {\n      \"type\": \"string\",\n      \"description\": \"The error type\"\n    },\n    \"Message\": {\n      \"type\": \"string\",\n      \"description\": \"The error message\"\n    },\n    \"Code\": {\n      \"type\": \"string\",\n      \"description\": \"The error code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-error-response-schema.json
tags: []
title: ErrorResponse
---
