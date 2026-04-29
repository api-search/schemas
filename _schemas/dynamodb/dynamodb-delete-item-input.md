---
description: ''
layout: schema
name: DeleteItemInput
properties_list:
- description: The name of the table from which to delete the item
  name: TableName
  type: string
- description: The primary key of the item to delete
  name: Key
  type: object
- description: A condition that must be satisfied for the deletion to succeed
  name: ConditionExpression
  type: string
- description: ''
  name: ExpressionAttributeNames
  type: object
- description: ''
  name: ExpressionAttributeValues
  type: object
- description: Whether to return the item attributes as they appeared before deletion
  name: ReturnValues
  type: string
- description: ''
  name: ReturnConsumedCapacity
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-delete-item-input-schema.json
slug: dynamodb-delete-item-input
source_filename: dynamodb-delete-item-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteItemInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table from which to delete the item\"\n    },\n    \"Key\": {\n      \"type\": \"object\",\n      \"description\": \"The primary key of the item to delete\"\n    },\n    \"ConditionExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A condition that must be satisfied for the deletion to succeed\"\n    },\n    \"ExpressionAttributeNames\": {\n      \"type\": \"object\"\n    },\n    \"ExpressionAttributeValues\": {\n      \"type\": \"object\"\n    },\n    \"ReturnValues\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to return the item attributes as they appeared before deletion\"\n    },\n    \"ReturnConsumedCapacity\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-delete-item-input-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: DeleteItemInput
---
