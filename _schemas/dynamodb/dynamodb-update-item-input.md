---
description: ''
layout: schema
name: UpdateItemInput
properties_list:
- description: The name of the table containing the item to update
  name: TableName
  type: string
- description: The primary key of the item to update
  name: Key
  type: object
- description: An expression that defines one or more attributes to be updated, the action to be performed on them, and new values for them
  name: UpdateExpression
  type: string
- description: A condition that must be satisfied for the update to succeed
  name: ConditionExpression
  type: string
- description: ''
  name: ExpressionAttributeNames
  type: object
- description: ''
  name: ExpressionAttributeValues
  type: object
- description: Whether to return the item attributes as they appeared before or after the update
  name: ReturnValues
  type: string
- description: ''
  name: ReturnConsumedCapacity
  type: string
- description: ''
  name: ReturnItemCollectionMetrics
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-update-item-input-schema.json
slug: dynamodb-update-item-input
source_filename: dynamodb-update-item-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateItemInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table containing the item to update\"\n    },\n    \"Key\": {\n      \"type\": \"object\",\n      \"description\": \"The primary key of the item to update\"\n    },\n    \"UpdateExpression\": {\n      \"type\": \"string\",\n      \"description\": \"An expression that defines one or more attributes to be updated, the action to be performed on them, and new values for them\"\n    },\n    \"ConditionExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A condition that must be satisfied for the update to succeed\"\n    },\n    \"ExpressionAttributeNames\": {\n      \"type\": \"object\"\n    },\n    \"ExpressionAttributeValues\": {\n      \"type\": \"object\"\n    },\n    \"ReturnValues\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"Whether to return the item attributes as they appeared before or after the update\"\n    },\n    \"ReturnConsumedCapacity\": {\n      \"type\": \"string\"\n    },\n    \"ReturnItemCollectionMetrics\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-update-item-input-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: UpdateItemInput
---
