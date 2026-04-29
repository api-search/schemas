---
description: GetItemInput schema from Amazon DynamoDB API
layout: schema
name: GetItemInput
properties_list:
- description: The name of the table containing the requested item
  name: TableName
  type: string
- description: A map of attribute names to AttributeValue objects for the primary key
  name: Key
  type: object
- description: A string that identifies attributes to retrieve
  name: ProjectionExpression
  type: string
- description: Determines the read consistency model
  name: ConsistentRead
  type: boolean
- description: Substitution tokens for attribute names in an expression
  name: ExpressionAttributeNames
  type: object
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-get-item-input-schema.json
slug: dynamodb-openapi-get-item-input
source_filename: dynamodb-openapi-get-item-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-get-item-input-schema.json\",\n  \"title\": \"GetItemInput\",\n  \"description\": \"GetItemInput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table containing the requested item\"\n    },\n    \"Key\": {\n      \"type\": \"object\",\n      \"description\": \"A map of attribute names to AttributeValue objects for the primary key\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AttributeValue\"\n      }\n    },\n    \"ProjectionExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A string that identifies attributes to retrieve\"\n    },\n    \"ConsistentRead\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Determines the read consistency model\"\n    },\n    \"ExpressionAttributeNames\": {\n      \"type\": \"object\",\n      \"description\": \"Substitution tokens for attribute names in an expression\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"TableName\",\n    \"Key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-get-item-input-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: GetItemInput
---
