---
description: BatchWriteItemInput schema from Amazon DynamoDB API
layout: schema
name: BatchWriteItemInput
properties_list:
- description: A map of table names to write requests
  name: RequestItems
  type: object
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-batch-write-item-input-schema.json
slug: dynamodb-openapi-batch-write-item-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-batch-write-item-input-schema.json\",\n  \"title\": \"BatchWriteItemInput\",\n  \"description\": \"BatchWriteItemInput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RequestItems\": {\n      \"type\": \"object\",\n      \"description\": \"A map of table names to write requests\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"PutRequest\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Item\": {\n                  \"type\": \"object\",\n                  \"additionalProperties\": {\n                    \"$ref\": \"#/components/schemas/AttributeValue\"\n                  }\n             \
  \   }\n              }\n            },\n            \"DeleteRequest\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Key\": {\n                  \"type\": \"object\",\n                  \"additionalProperties\": {\n                    \"$ref\": \"#/components/schemas/AttributeValue\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"RequestItems\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-batch-write-item-input-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: BatchWriteItemInput
---
