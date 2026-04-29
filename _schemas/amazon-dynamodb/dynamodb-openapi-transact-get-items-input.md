---
description: TransactGetItemsInput schema from Amazon DynamoDB API
layout: schema
name: TransactGetItemsInput
properties_list:
- description: An ordered array of up to 100 TransactGetItem objects
  name: TransactItems
  type: array
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-transact-get-items-input-schema.json
slug: dynamodb-openapi-transact-get-items-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-transact-get-items-input-schema.json\",\n  \"title\": \"TransactGetItemsInput\",\n  \"description\": \"TransactGetItemsInput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransactItems\": {\n      \"type\": \"array\",\n      \"description\": \"An ordered array of up to 100 TransactGetItem objects\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Get\": {\n            \"type\": \"object\",\n            \"required\": [\n              \"TableName\",\n              \"Key\"\n            ],\n            \"properties\": {\n              \"TableName\": {\n                \"type\": \"string\"\n              },\n              \"Key\": {\n                \"type\": \"object\",\n                \"additionalProperties\"\
  : {\n                  \"$ref\": \"#/components/schemas/AttributeValue\"\n                }\n              },\n              \"ProjectionExpression\": {\n                \"type\": \"string\"\n              },\n              \"ExpressionAttributeNames\": {\n                \"type\": \"object\",\n                \"additionalProperties\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      },\n      \"maxItems\": 100\n    }\n  },\n  \"required\": [\n    \"TransactItems\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-transact-get-items-input-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: TransactGetItemsInput
---
