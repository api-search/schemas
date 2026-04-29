---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: The exception type
  name: __type
  type: string
- description: A human-readable description of the error
  name: message
  type: string
- description: A human-readable description of the error (alternative casing)
  name: Message
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-error-response-schema.json
slug: dynamodb-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"__type\": {\n      \"type\": \"string\",\n      \"description\": \"The exception type\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the error\"\n    },\n    \"Message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the error (alternative casing)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-error-response-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ErrorResponse
---
