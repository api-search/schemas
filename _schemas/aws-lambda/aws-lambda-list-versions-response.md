---
description: Paginated list of function versions
layout: schema
name: ListVersionsResponse
properties_list:
- description: Pagination token for the next page
  name: NextMarker
  type: string
- description: ''
  name: Versions
  type: array
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-list-versions-response-schema.json
slug: aws-lambda-list-versions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListVersionsResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of function versions\",\n  \"properties\": {\n    \"NextMarker\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for the next page\"\n    },\n    \"Versions\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-list-versions-response-schema.json
tags: []
title: ListVersionsResponse
---
