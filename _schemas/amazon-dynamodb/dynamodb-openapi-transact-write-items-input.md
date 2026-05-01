---
description: TransactWriteItemsInput schema from Amazon DynamoDB API
layout: schema
name: TransactWriteItemsInput
properties_list:
- description: An ordered array of up to 100 TransactWriteItem objects
  name: TransactItems
  type: array
- description: A unique identifier for the client request to ensure idempotency
  name: ClientRequestToken
  type: string
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-transact-write-items-input-schema.json
slug: dynamodb-openapi-transact-write-items-input
source_filename: dynamodb-openapi-transact-write-items-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-transact-write-items-input-schema.json\",\n  \"title\": \"TransactWriteItemsInput\",\n  \"description\": \"TransactWriteItemsInput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransactItems\": {\n      \"type\": \"array\",\n      \"description\": \"An ordered array of up to 100 TransactWriteItem objects\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"ConditionCheck\": {\n            \"type\": \"object\",\n            \"description\": \"A request to perform a check item operation\"\n          },\n          \"Put\": {\n            \"type\": \"object\",\n            \"description\": \"A request to perform a PutItem operation\"\n          },\n          \"Delete\": {\n            \"type\": \"object\",\n\
  \            \"description\": \"A request to perform a DeleteItem operation\"\n          },\n          \"Update\": {\n            \"type\": \"object\",\n            \"description\": \"A request to perform an UpdateItem operation\"\n          }\n        }\n      },\n      \"maxItems\": 100\n    },\n    \"ClientRequestToken\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the client request to ensure idempotency\",\n      \"minLength\": 1,\n      \"maxLength\": 36\n    }\n  },\n  \"required\": [\n    \"TransactItems\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-transact-write-items-input-schema.json
tags:
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: TransactWriteItemsInput
---
