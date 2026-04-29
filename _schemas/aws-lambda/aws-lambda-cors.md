---
description: Cross-origin resource sharing (CORS) settings for a function URL
layout: schema
name: Cors
properties_list:
- description: Whether to allow cookies or other credentials
  name: AllowCredentials
  type: boolean
- description: The HTTP headers allowed in requests
  name: AllowHeaders
  type: array
- description: The HTTP methods allowed
  name: AllowMethods
  type: array
- description: The origins allowed to access the function URL
  name: AllowOrigins
  type: array
- description: The HTTP headers exposed in the response
  name: ExposeHeaders
  type: array
- description: Maximum time in seconds that a browser can cache results of a preflight request
  name: MaxAge
  type: integer
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-cors-schema.json
slug: aws-lambda-cors
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Cors\",\n  \"type\": \"object\",\n  \"description\": \"Cross-origin resource sharing (CORS) settings for a function URL\",\n  \"properties\": {\n    \"AllowCredentials\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to allow cookies or other credentials\"\n    },\n    \"AllowHeaders\": {\n      \"type\": \"array\",\n      \"description\": \"The HTTP headers allowed in requests\"\n    },\n    \"AllowMethods\": {\n      \"type\": \"array\",\n      \"description\": \"The HTTP methods allowed\"\n    },\n    \"AllowOrigins\": {\n      \"type\": \"array\",\n      \"description\": \"The origins allowed to access the function URL\"\n    },\n    \"ExposeHeaders\": {\n      \"type\": \"array\",\n      \"description\": \"The HTTP headers exposed in the response\"\n    },\n    \"MaxAge\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum time in seconds that a browser\
  \ can cache results of a preflight request\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-cors-schema.json
tags: []
title: Cors
---
