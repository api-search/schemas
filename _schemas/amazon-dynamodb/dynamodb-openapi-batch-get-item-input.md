---
description: BatchGetItemInput schema from Amazon DynamoDB API
layout: schema
name: BatchGetItemInput
properties_list:
- description: A map of table names to keys and attributes to retrieve
  name: RequestItems
  type: object
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-batch-get-item-input-schema.json
slug: dynamodb-openapi-batch-get-item-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-batch-get-item-input-schema.json\",\n  \"title\": \"BatchGetItemInput\",\n  \"description\": \"BatchGetItemInput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RequestItems\": {\n      \"type\": \"object\",\n      \"description\": \"A map of table names to keys and attributes to retrieve\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Keys\": {\n            \"type\": \"array\",\n            \"description\": \"The primary keys for items to retrieve\",\n            \"items\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"$ref\": \"#/components/schemas/AttributeValue\"\n              }\n            }\n          },\n          \"ProjectionExpression\"\
  : {\n            \"type\": \"string\"\n          },\n          \"ConsistentRead\": {\n            \"type\": \"boolean\"\n          },\n          \"ExpressionAttributeNames\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"RequestItems\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-batch-get-item-input-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: BatchGetItemInput
---
