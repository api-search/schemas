---
description: ''
layout: schema
name: GetItemInput
properties_list:
- description: The name of the table containing the requested item
  name: TableName
  type: string
- description: A map of attribute names to AttributeValue objects, representing the primary key of the item to retrieve
  name: Key
  type: object
- description: A string that identifies one or more attributes to retrieve from the table
  name: ProjectionExpression
  type: string
- description: One or more substitution tokens for attribute names in an expression
  name: ExpressionAttributeNames
  type: object
- description: If set to true, the operation uses strongly consistent reads; otherwise, eventually consistent reads are used
  name: ConsistentRead
  type: boolean
- description: ''
  name: ReturnConsumedCapacity
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-get-item-input-schema.json
slug: dynamodb-get-item-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetItemInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table containing the requested item\"\n    },\n    \"Key\": {\n      \"type\": \"object\",\n      \"description\": \"A map of attribute names to AttributeValue objects, representing the primary key of the item to retrieve\"\n    },\n    \"ProjectionExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A string that identifies one or more attributes to retrieve from the table\"\n    },\n    \"ExpressionAttributeNames\": {\n      \"type\": \"object\",\n      \"description\": \"One or more substitution tokens for attribute names in an expression\"\n    },\n    \"ConsistentRead\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to true, the operation uses strongly consistent reads; otherwise, eventually consistent\
  \ reads are used\"\n    },\n    \"ReturnConsumedCapacity\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-get-item-input-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: GetItemInput
---
