---
description: ''
layout: schema
name: BatchExecuteStatementInput
properties_list:
- description: The list of PartiQL statements representing the batch to run
  name: Statements
  type: array
- description: ''
  name: ReturnConsumedCapacity
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-batch-execute-statement-input-schema.json
slug: dynamodb-batch-execute-statement-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchExecuteStatementInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Statements\": {\n      \"type\": \"array\",\n      \"description\": \"The list of PartiQL statements representing the batch to run\"\n    },\n    \"ReturnConsumedCapacity\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-batch-execute-statement-input-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: BatchExecuteStatementInput
---
