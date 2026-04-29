---
description: UpdateItemInput schema from Amazon DynamoDB API
layout: schema
name: UpdateItemInput
properties_list:
- description: The name of the table containing the item to update
  name: TableName
  type: string
- description: The primary key of the item to be updated
  name: Key
  type: object
- description: An expression that defines attributes to be updated
  name: UpdateExpression
  type: string
- description: A condition that must be satisfied for the update to succeed
  name: ConditionExpression
  type: string
- description: Substitution tokens for attribute names in an expression
  name: ExpressionAttributeNames
  type: object
- description: Values that can be substituted in an expression
  name: ExpressionAttributeValues
  type: object
- description: Determines the return values after the operation
  name: ReturnValues
  type: string
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-update-item-input-schema.json
slug: dynamodb-openapi-update-item-input
source_filename: dynamodb-openapi-update-item-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-update-item-input-schema.json\",\n  \"title\": \"UpdateItemInput\",\n  \"description\": \"UpdateItemInput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table containing the item to update\"\n    },\n    \"Key\": {\n      \"type\": \"object\",\n      \"description\": \"The primary key of the item to be updated\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AttributeValue\"\n      }\n    },\n    \"UpdateExpression\": {\n      \"type\": \"string\",\n      \"description\": \"An expression that defines attributes to be updated\"\n    },\n    \"ConditionExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A condition\
  \ that must be satisfied for the update to succeed\"\n    },\n    \"ExpressionAttributeNames\": {\n      \"type\": \"object\",\n      \"description\": \"Substitution tokens for attribute names in an expression\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"ExpressionAttributeValues\": {\n      \"type\": \"object\",\n      \"description\": \"Values that can be substituted in an expression\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AttributeValue\"\n      }\n    },\n    \"ReturnValues\": {\n      \"type\": \"string\",\n      \"description\": \"Determines the return values after the operation\",\n      \"enum\": [\n        \"NONE\",\n        \"UPDATED_OLD\",\n        \"ALL_OLD\",\n        \"UPDATED_NEW\",\n        \"ALL_NEW\"\n      ]\n    }\n  },\n  \"required\": [\n    \"TableName\",\n    \"Key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-update-item-input-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: UpdateItemInput
---
