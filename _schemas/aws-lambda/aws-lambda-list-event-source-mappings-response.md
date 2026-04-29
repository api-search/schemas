---
description: Paginated list of event source mappings
layout: schema
name: ListEventSourceMappingsResponse
properties_list:
- description: Pagination token
  name: NextMarker
  type: string
- description: ''
  name: EventSourceMappings
  type: array
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-list-event-source-mappings-response-schema.json
slug: aws-lambda-list-event-source-mappings-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListEventSourceMappingsResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of event source mappings\",\n  \"properties\": {\n    \"NextMarker\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token\"\n    },\n    \"EventSourceMappings\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-list-event-source-mappings-response-schema.json
tags: []
title: ListEventSourceMappingsResponse
---
