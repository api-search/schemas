---
description: Paginated list of aliases
layout: schema
name: ListAliasesResponse
properties_list:
- description: Pagination token for the next page
  name: NextMarker
  type: string
- description: ''
  name: Aliases
  type: array
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-list-aliases-response-schema.json
slug: aws-lambda-list-aliases-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListAliasesResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of aliases\",\n  \"properties\": {\n    \"NextMarker\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for the next page\"\n    },\n    \"Aliases\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-list-aliases-response-schema.json
tags: []
title: ListAliasesResponse
---
