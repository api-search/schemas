---
description: Paginated list of Lambda functions
layout: schema
name: ListFunctionsResponse
properties_list:
- description: Pagination token for the next page of results
  name: NextMarker
  type: string
- description: ''
  name: Functions
  type: array
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-list-functions-response-schema.json
slug: aws-lambda-list-functions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListFunctionsResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of Lambda functions\",\n  \"properties\": {\n    \"NextMarker\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for the next page of results\"\n    },\n    \"Functions\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-list-functions-response-schema.json
tags: []
title: ListFunctionsResponse
---
