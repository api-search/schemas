---
description: PutItemInput schema from Amazon DynamoDB API
layout: schema
name: PutItemInput
properties_list:
- description: The name of the table to contain the item
  name: TableName
  type: string
- description: A map of attribute name to attribute values, representing the item
  name: Item
  type: object
- description: A condition that must be satisfied for a put to succeed
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
schema_file: json-schema/dynamodb-openapi-put-item-input-schema.json
slug: dynamodb-openapi-put-item-input
source_filename: dynamodb-openapi-put-item-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-put-item-input-schema.json\",\n  \"title\": \"PutItemInput\",\n  \"description\": \"PutItemInput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table to contain the item\"\n    },\n    \"Item\": {\n      \"type\": \"object\",\n      \"description\": \"A map of attribute name to attribute values, representing the item\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AttributeValue\"\n      }\n    },\n    \"ConditionExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A condition that must be satisfied for a put to succeed\"\n    },\n    \"ExpressionAttributeNames\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Substitution tokens for attribute names in an expression\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"ExpressionAttributeValues\": {\n      \"type\": \"object\",\n      \"description\": \"Values that can be substituted in an expression\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AttributeValue\"\n      }\n    },\n    \"ReturnValues\": {\n      \"type\": \"string\",\n      \"description\": \"Determines the return values after the operation\",\n      \"enum\": [\n        \"NONE\",\n        \"ALL_OLD\"\n      ]\n    }\n  },\n  \"required\": [\n    \"TableName\",\n    \"Item\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-put-item-input-schema.json
tags:
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: PutItemInput
---
