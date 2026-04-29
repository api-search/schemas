---
description: ''
layout: schema
name: PutItemInput
properties_list:
- description: The name of the table to contain the item
  name: TableName
  type: string
- description: A map of attribute name/value pairs, one for each attribute. Only the primary key attributes are required, but you can optionally provide other attribute name-value pairs.
  name: Item
  type: object
- description: A condition that must be satisfied in order for a conditional PutItem operation to succeed
  name: ConditionExpression
  type: string
- description: One or more substitution tokens for attribute names in an expression
  name: ExpressionAttributeNames
  type: object
- description: One or more values that can be substituted in an expression
  name: ExpressionAttributeValues
  type: object
- description: Whether to return the item attributes as they appeared before the PutItem
  name: ReturnValues
  type: string
- description: Determines the level of detail about provisioned throughput consumption
  name: ReturnConsumedCapacity
  type: string
- description: Determines whether item collection metrics are returned
  name: ReturnItemCollectionMetrics
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-put-item-input-schema.json
slug: dynamodb-put-item-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PutItemInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table to contain the item\"\n    },\n    \"Item\": {\n      \"type\": \"object\",\n      \"description\": \"A map of attribute name/value pairs, one for each attribute. Only the primary key attributes are required, but you can optionally provide other attribute name-value pairs.\"\n    },\n    \"ConditionExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A condition that must be satisfied in order for a conditional PutItem operation to succeed\"\n    },\n    \"ExpressionAttributeNames\": {\n      \"type\": \"object\",\n      \"description\": \"One or more substitution tokens for attribute names in an expression\"\n    },\n    \"ExpressionAttributeValues\": {\n      \"type\": \"object\",\n      \"description\": \"One or\
  \ more values that can be substituted in an expression\"\n    },\n    \"ReturnValues\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to return the item attributes as they appeared before the PutItem\"\n    },\n    \"ReturnConsumedCapacity\": {\n      \"type\": \"string\",\n      \"description\": \"Determines the level of detail about provisioned throughput consumption\"\n    },\n    \"ReturnItemCollectionMetrics\": {\n      \"type\": \"string\",\n      \"description\": \"Determines whether item collection metrics are returned\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-put-item-input-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: PutItemInput
---
