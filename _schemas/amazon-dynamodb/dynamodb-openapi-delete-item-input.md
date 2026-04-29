---
description: DeleteItemInput schema from Amazon DynamoDB API
layout: schema
name: DeleteItemInput
properties_list:
- description: The name of the table from which to delete the item
  name: TableName
  type: string
- description: A map of attribute names to AttributeValue objects for the primary key
  name: Key
  type: object
- description: A condition that must be satisfied for the delete to succeed
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
schema_file: json-schema/dynamodb-openapi-delete-item-input-schema.json
slug: dynamodb-openapi-delete-item-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-delete-item-input-schema.json\",\n  \"title\": \"DeleteItemInput\",\n  \"description\": \"DeleteItemInput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table from which to delete the item\"\n    },\n    \"Key\": {\n      \"type\": \"object\",\n      \"description\": \"A map of attribute names to AttributeValue objects for the primary key\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AttributeValue\"\n      }\n    },\n    \"ConditionExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A condition that must be satisfied for the delete to succeed\"\n    },\n    \"ExpressionAttributeNames\": {\n      \"type\": \"\
  object\",\n      \"description\": \"Substitution tokens for attribute names in an expression\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"ExpressionAttributeValues\": {\n      \"type\": \"object\",\n      \"description\": \"Values that can be substituted in an expression\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AttributeValue\"\n      }\n    },\n    \"ReturnValues\": {\n      \"type\": \"string\",\n      \"description\": \"Determines the return values after the operation\",\n      \"enum\": [\n        \"NONE\",\n        \"ALL_OLD\"\n      ]\n    }\n  },\n  \"required\": [\n    \"TableName\",\n    \"Key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-delete-item-input-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: DeleteItemInput
---
