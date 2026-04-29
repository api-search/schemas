---
description: ''
layout: schema
name: ConsumedCapacity
properties_list:
- description: The name of the table that was affected by the operation
  name: TableName
  type: string
- description: The total number of capacity units consumed by the operation
  name: CapacityUnits
  type: number
- description: The total number of read capacity units consumed
  name: ReadCapacityUnits
  type: number
- description: The total number of write capacity units consumed
  name: WriteCapacityUnits
  type: number
- description: ''
  name: Table
  type: object
- description: ''
  name: LocalSecondaryIndexes
  type: object
- description: ''
  name: GlobalSecondaryIndexes
  type: object
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-consumed-capacity-schema.json
slug: dynamodb-consumed-capacity
source_filename: dynamodb-consumed-capacity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConsumedCapacity\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table that was affected by the operation\"\n    },\n    \"CapacityUnits\": {\n      \"type\": \"number\",\n      \"description\": \"The total number of capacity units consumed by the operation\"\n    },\n    \"ReadCapacityUnits\": {\n      \"type\": \"number\",\n      \"description\": \"The total number of read capacity units consumed\"\n    },\n    \"WriteCapacityUnits\": {\n      \"type\": \"number\",\n      \"description\": \"The total number of write capacity units consumed\"\n    },\n    \"Table\": {\n      \"type\": \"object\"\n    },\n    \"LocalSecondaryIndexes\": {\n      \"type\": \"object\"\n    },\n    \"GlobalSecondaryIndexes\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-consumed-capacity-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ConsumedCapacity
---
