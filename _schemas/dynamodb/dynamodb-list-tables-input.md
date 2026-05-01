---
description: ''
layout: schema
name: ListTablesInput
properties_list:
- description: The first table name that this operation will evaluate. Use the value returned for LastEvaluatedTableName in a previous operation.
  name: ExclusiveStartTableName
  type: string
- description: Maximum number of table names to return (1-100)
  name: Limit
  type: integer
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-list-tables-input-schema.json
slug: dynamodb-list-tables-input
source_filename: dynamodb-list-tables-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListTablesInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ExclusiveStartTableName\": {\n      \"type\": \"string\",\n      \"description\": \"The first table name that this operation will evaluate. Use the value returned for LastEvaluatedTableName in a previous operation.\"\n    },\n    \"Limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of table names to return (1-100)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-list-tables-input-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ListTablesInput
---
