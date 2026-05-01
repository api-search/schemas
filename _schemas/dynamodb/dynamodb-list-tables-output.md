---
description: ''
layout: schema
name: ListTablesOutput
properties_list:
- description: The names of the tables associated with the current account
  name: TableNames
  type: array
- description: The name of the last table in the current page of results. Use this value as ExclusiveStartTableName for the next request.
  name: LastEvaluatedTableName
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-list-tables-output-schema.json
slug: dynamodb-list-tables-output
source_filename: dynamodb-list-tables-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListTablesOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableNames\": {\n      \"type\": \"array\",\n      \"description\": \"The names of the tables associated with the current account\"\n    },\n    \"LastEvaluatedTableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the last table in the current page of results. Use this value as ExclusiveStartTableName for the next request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-list-tables-output-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ListTablesOutput
---
