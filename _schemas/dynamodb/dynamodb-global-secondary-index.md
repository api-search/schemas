---
description: ''
layout: schema
name: GlobalSecondaryIndex
properties_list:
- description: The name of the global secondary index
  name: IndexName
  type: string
- description: The key schema for the global secondary index
  name: KeySchema
  type: array
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-global-secondary-index-schema.json
slug: dynamodb-global-secondary-index
source_filename: dynamodb-global-secondary-index-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GlobalSecondaryIndex\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IndexName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the global secondary index\"\n    },\n    \"KeySchema\": {\n      \"type\": \"array\",\n      \"description\": \"The key schema for the global secondary index\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-global-secondary-index-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: GlobalSecondaryIndex
---
