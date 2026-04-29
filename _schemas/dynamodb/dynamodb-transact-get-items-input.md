---
description: ''
layout: schema
name: TransactGetItemsInput
properties_list:
- description: An ordered array of up to 100 TransactGetItem objects
  name: TransactItems
  type: array
- description: ''
  name: ReturnConsumedCapacity
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-transact-get-items-input-schema.json
slug: dynamodb-transact-get-items-input
source_filename: dynamodb-transact-get-items-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransactGetItemsInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransactItems\": {\n      \"type\": \"array\",\n      \"description\": \"An ordered array of up to 100 TransactGetItem objects\"\n    },\n    \"ReturnConsumedCapacity\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-transact-get-items-input-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: TransactGetItemsInput
---
