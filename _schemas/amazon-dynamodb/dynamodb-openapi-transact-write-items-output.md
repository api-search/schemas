---
description: TransactWriteItemsOutput schema from Amazon DynamoDB API
layout: schema
name: TransactWriteItemsOutput
properties_list:
- description: A list of tables affected by the TransactWriteItems call
  name: ItemCollectionMetrics
  type: object
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-transact-write-items-output-schema.json
slug: dynamodb-openapi-transact-write-items-output
source_filename: dynamodb-openapi-transact-write-items-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-transact-write-items-output-schema.json\",\n  \"title\": \"TransactWriteItemsOutput\",\n  \"description\": \"TransactWriteItemsOutput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ItemCollectionMetrics\": {\n      \"type\": \"object\",\n      \"description\": \"A list of tables affected by the TransactWriteItems call\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-transact-write-items-output-schema.json
tags:
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: TransactWriteItemsOutput
---
