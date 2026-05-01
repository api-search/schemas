---
description: QueryInput schema from Amazon DynamoDB API
layout: schema
name: QueryInput
properties_list:
- description: The name of the table to query
  name: TableName
  type: string
- description: The name of a secondary index to query
  name: IndexName
  type: string
- description: The condition that specifies the key values for items to be retrieved
  name: KeyConditionExpression
  type: string
- description: A string that contains conditions for filtering the query results
  name: FilterExpression
  type: string
- description: A string that identifies attributes to retrieve
  name: ProjectionExpression
  type: string
- description: Substitution tokens for attribute names in an expression
  name: ExpressionAttributeNames
  type: object
- description: Values that can be substituted in an expression
  name: ExpressionAttributeValues
  type: object
- description: Specifies the order for index traversal (true=ascending, false=descending)
  name: ScanIndexForward
  type: boolean
- description: The maximum number of items to evaluate
  name: Limit
  type: integer
- description: Determines the read consistency model
  name: ConsistentRead
  type: boolean
- description: The primary key of the first item that this operation evaluates
  name: ExclusiveStartKey
  type: object
- description: The attributes to be returned in the result
  name: Select
  type: string
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-query-input-schema.json
slug: dynamodb-openapi-query-input
source_filename: dynamodb-openapi-query-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-query-input-schema.json\",\n  \"title\": \"QueryInput\",\n  \"description\": \"QueryInput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table to query\"\n    },\n    \"IndexName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of a secondary index to query\"\n    },\n    \"KeyConditionExpression\": {\n      \"type\": \"string\",\n      \"description\": \"The condition that specifies the key values for items to be retrieved\"\n    },\n    \"FilterExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A string that contains conditions for filtering the query results\"\n    },\n    \"ProjectionExpression\": {\n      \"type\": \"\
  string\",\n      \"description\": \"A string that identifies attributes to retrieve\"\n    },\n    \"ExpressionAttributeNames\": {\n      \"type\": \"object\",\n      \"description\": \"Substitution tokens for attribute names in an expression\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"ExpressionAttributeValues\": {\n      \"type\": \"object\",\n      \"description\": \"Values that can be substituted in an expression\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AttributeValue\"\n      }\n    },\n    \"ScanIndexForward\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies the order for index traversal (true=ascending, false=descending)\",\n      \"default\": true\n    },\n    \"Limit\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of items to evaluate\",\n      \"minimum\": 1\n    },\n    \"ConsistentRead\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Determines the read consistency model\"\n    },\n    \"ExclusiveStartKey\": {\n      \"type\": \"object\",\n      \"description\": \"The primary key of the first item that this operation evaluates\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AttributeValue\"\n      }\n    },\n    \"Select\": {\n      \"type\": \"string\",\n      \"description\": \"The attributes to be returned in the result\",\n      \"enum\": [\n        \"ALL_ATTRIBUTES\",\n        \"ALL_PROJECTED_ATTRIBUTES\",\n        \"COUNT\",\n        \"SPECIFIC_ATTRIBUTES\"\n      ]\n    }\n  },\n  \"required\": [\n    \"TableName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-query-input-schema.json
tags:
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: QueryInput
---
