---
description: BatchWriteItemOutput schema from Amazon DynamoDB API
layout: schema
name: BatchWriteItemOutput
properties_list:
- description: A map of tables and requests against those tables that were not processed
  name: UnprocessedItems
  type: object
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-batch-write-item-output-schema.json
slug: dynamodb-openapi-batch-write-item-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-batch-write-item-output-schema.json\",\n  \"title\": \"BatchWriteItemOutput\",\n  \"description\": \"BatchWriteItemOutput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UnprocessedItems\": {\n      \"type\": \"object\",\n      \"description\": \"A map of tables and requests against those tables that were not processed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-batch-write-item-output-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: BatchWriteItemOutput
---
