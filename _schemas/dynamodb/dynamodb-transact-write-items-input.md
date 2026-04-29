---
description: ''
layout: schema
name: TransactWriteItemsInput
properties_list:
- description: An ordered array of up to 100 TransactWriteItem objects
  name: TransactItems
  type: array
- description: Unique identifier for the idempotency of the request
  name: ClientRequestToken
  type: string
- description: ''
  name: ReturnConsumedCapacity
  type: string
- description: ''
  name: ReturnItemCollectionMetrics
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-transact-write-items-input-schema.json
slug: dynamodb-transact-write-items-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransactWriteItemsInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransactItems\": {\n      \"type\": \"array\",\n      \"description\": \"An ordered array of up to 100 TransactWriteItem objects\"\n    },\n    \"ClientRequestToken\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the idempotency of the request\"\n    },\n    \"ReturnConsumedCapacity\": {\n      \"type\": \"string\"\n    },\n    \"ReturnItemCollectionMetrics\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-transact-write-items-input-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: TransactWriteItemsInput
---
