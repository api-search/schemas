---
description: ''
layout: schema
name: BatchGetItemInput
properties_list:
- description: A map of one or more table names and, for each table, a map that describes one or more items to retrieve from that table
  name: RequestItems
  type: object
- description: ''
  name: ReturnConsumedCapacity
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-batch-get-item-input-schema.json
slug: dynamodb-batch-get-item-input
source_filename: dynamodb-batch-get-item-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchGetItemInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RequestItems\": {\n      \"type\": \"object\",\n      \"description\": \"A map of one or more table names and, for each table, a map that describes one or more items to retrieve from that table\"\n    },\n    \"ReturnConsumedCapacity\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-batch-get-item-input-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: BatchGetItemInput
---
