---
description: ''
layout: schema
name: ExecuteTransactionInput
properties_list:
- description: The list of PartiQL statements representing the transaction to run
  name: TransactStatements
  type: array
- description: Unique identifier for idempotency
  name: ClientRequestToken
  type: string
- description: ''
  name: ReturnConsumedCapacity
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-execute-transaction-input-schema.json
slug: dynamodb-execute-transaction-input
source_filename: dynamodb-execute-transaction-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExecuteTransactionInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransactStatements\": {\n      \"type\": \"array\",\n      \"description\": \"The list of PartiQL statements representing the transaction to run\"\n    },\n    \"ClientRequestToken\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for idempotency\"\n    },\n    \"ReturnConsumedCapacity\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-execute-transaction-input-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ExecuteTransactionInput
---
