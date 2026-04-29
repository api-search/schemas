---
description: ''
layout: schema
name: BatchGetItemOutput
properties_list:
- description: A map of table name to a list of items
  name: Responses
  type: object
- description: A map of tables and their respective keys that were not processed. Retry these using exponential backoff.
  name: UnprocessedKeys
  type: object
- description: ''
  name: ConsumedCapacity
  type: array
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-batch-get-item-output-schema.json
slug: dynamodb-batch-get-item-output
source_filename: dynamodb-batch-get-item-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchGetItemOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Responses\": {\n      \"type\": \"object\",\n      \"description\": \"A map of table name to a list of items\"\n    },\n    \"UnprocessedKeys\": {\n      \"type\": \"object\",\n      \"description\": \"A map of tables and their respective keys that were not processed. Retry these using exponential backoff.\"\n    },\n    \"ConsumedCapacity\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-batch-get-item-output-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: BatchGetItemOutput
---
