---
description: ''
layout: schema
name: BatchExecuteStatementOutput
properties_list:
- description: ''
  name: Responses
  type: array
- description: ''
  name: ConsumedCapacity
  type: array
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-batch-execute-statement-output-schema.json
slug: dynamodb-batch-execute-statement-output
source_filename: dynamodb-batch-execute-statement-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchExecuteStatementOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Responses\": {\n      \"type\": \"array\"\n    },\n    \"ConsumedCapacity\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-batch-execute-statement-output-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: BatchExecuteStatementOutput
---
