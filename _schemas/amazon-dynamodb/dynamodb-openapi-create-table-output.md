---
description: CreateTableOutput schema from Amazon DynamoDB API
layout: schema
name: CreateTableOutput
properties_list:
- description: ''
  name: TableDescription
  type: object
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-create-table-output-schema.json
slug: dynamodb-openapi-create-table-output
source_filename: dynamodb-openapi-create-table-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-create-table-output-schema.json\",\n  \"title\": \"CreateTableOutput\",\n  \"description\": \"CreateTableOutput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableDescription\": {\n      \"$ref\": \"#/components/schemas/TableDescription\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-create-table-output-schema.json
tags:
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: CreateTableOutput
---
