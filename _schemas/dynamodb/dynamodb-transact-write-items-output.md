---
description: ''
layout: schema
name: TransactWriteItemsOutput
properties_list:
- description: ''
  name: ConsumedCapacity
  type: array
- description: ''
  name: ItemCollectionMetrics
  type: object
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-transact-write-items-output-schema.json
slug: dynamodb-transact-write-items-output
source_filename: dynamodb-transact-write-items-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransactWriteItemsOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConsumedCapacity\": {\n      \"type\": \"array\"\n    },\n    \"ItemCollectionMetrics\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-transact-write-items-output-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: TransactWriteItemsOutput
---
