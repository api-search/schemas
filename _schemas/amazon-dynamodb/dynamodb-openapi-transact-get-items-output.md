---
description: TransactGetItemsOutput schema from Amazon DynamoDB API
layout: schema
name: TransactGetItemsOutput
properties_list:
- description: An ordered array of up to 100 ItemResponse objects
  name: Responses
  type: array
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-transact-get-items-output-schema.json
slug: dynamodb-openapi-transact-get-items-output
source_filename: dynamodb-openapi-transact-get-items-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-transact-get-items-output-schema.json\",\n  \"title\": \"TransactGetItemsOutput\",\n  \"description\": \"TransactGetItemsOutput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Responses\": {\n      \"type\": \"array\",\n      \"description\": \"An ordered array of up to 100 ItemResponse objects\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Item\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"$ref\": \"#/components/schemas/AttributeValue\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-transact-get-items-output-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: TransactGetItemsOutput
---
