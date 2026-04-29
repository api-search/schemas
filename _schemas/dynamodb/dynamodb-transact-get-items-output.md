---
description: ''
layout: schema
name: TransactGetItemsOutput
properties_list:
- description: An ordered array of up to 100 ItemResponse objects
  name: Responses
  type: array
- description: ''
  name: ConsumedCapacity
  type: array
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-transact-get-items-output-schema.json
slug: dynamodb-transact-get-items-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransactGetItemsOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Responses\": {\n      \"type\": \"array\",\n      \"description\": \"An ordered array of up to 100 ItemResponse objects\"\n    },\n    \"ConsumedCapacity\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-transact-get-items-output-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: TransactGetItemsOutput
---
