---
description: ''
layout: schema
name: ExecuteStatementInput
properties_list:
- description: The PartiQL statement representing the operation to run
  name: Statement
  type: string
- description: The parameters for the PartiQL statement
  name: Parameters
  type: array
- description: The consistency of a read operation
  name: ConsistentRead
  type: boolean
- description: Set this value to get remaining results
  name: NextToken
  type: string
- description: ''
  name: ReturnConsumedCapacity
  type: string
- description: The maximum number of items to evaluate
  name: Limit
  type: integer
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-execute-statement-input-schema.json
slug: dynamodb-execute-statement-input
source_filename: dynamodb-execute-statement-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExecuteStatementInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Statement\": {\n      \"type\": \"string\",\n      \"description\": \"The PartiQL statement representing the operation to run\"\n    },\n    \"Parameters\": {\n      \"type\": \"array\",\n      \"description\": \"The parameters for the PartiQL statement\"\n    },\n    \"ConsistentRead\": {\n      \"type\": \"boolean\",\n      \"description\": \"The consistency of a read operation\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Set this value to get remaining results\"\n    },\n    \"ReturnConsumedCapacity\": {\n      \"type\": \"string\"\n    },\n    \"Limit\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of items to evaluate\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-execute-statement-input-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ExecuteStatementInput
---
