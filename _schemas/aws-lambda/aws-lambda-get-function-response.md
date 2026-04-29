---
description: Response containing function details and code location
layout: schema
name: GetFunctionResponse
properties_list:
- description: The deployment package of the function
  name: Code
  type: object
- description: The function's tags
  name: Tags
  type: object
- description: ''
  name: Concurrency
  type: object
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-get-function-response-schema.json
slug: aws-lambda-get-function-response
source_filename: aws-lambda-get-function-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetFunctionResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response containing function details and code location\",\n  \"properties\": {\n    \"Code\": {\n      \"type\": \"object\",\n      \"description\": \"The deployment package of the function\"\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"description\": \"The function's tags\"\n    },\n    \"Concurrency\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-get-function-response-schema.json
tags: []
title: GetFunctionResponse
---
