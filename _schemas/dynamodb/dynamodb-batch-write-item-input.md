---
description: ''
layout: schema
name: BatchWriteItemInput
properties_list:
- description: A map of one or more table names and, for each table, a list of operations to perform (PutRequest or DeleteRequest)
  name: RequestItems
  type: object
- description: ''
  name: ReturnConsumedCapacity
  type: string
- description: ''
  name: ReturnItemCollectionMetrics
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-batch-write-item-input-schema.json
slug: dynamodb-batch-write-item-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchWriteItemInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RequestItems\": {\n      \"type\": \"object\",\n      \"description\": \"A map of one or more table names and, for each table, a list of operations to perform (PutRequest or DeleteRequest)\"\n    },\n    \"ReturnConsumedCapacity\": {\n      \"type\": \"string\"\n    },\n    \"ReturnItemCollectionMetrics\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-batch-write-item-input-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: BatchWriteItemInput
---
