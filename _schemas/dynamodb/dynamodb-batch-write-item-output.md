---
description: ''
layout: schema
name: BatchWriteItemOutput
properties_list:
- description: A map of unprocessed items to retry
  name: UnprocessedItems
  type: object
- description: ''
  name: ItemCollectionMetrics
  type: object
- description: ''
  name: ConsumedCapacity
  type: array
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-batch-write-item-output-schema.json
slug: dynamodb-batch-write-item-output
source_filename: dynamodb-batch-write-item-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchWriteItemOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UnprocessedItems\": {\n      \"type\": \"object\",\n      \"description\": \"A map of unprocessed items to retry\"\n    },\n    \"ItemCollectionMetrics\": {\n      \"type\": \"object\"\n    },\n    \"ConsumedCapacity\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-batch-write-item-output-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: BatchWriteItemOutput
---
