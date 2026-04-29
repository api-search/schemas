---
description: ''
layout: schema
name: ExecuteStatementOutput
properties_list:
- description: ''
  name: Items
  type: array
- description: ''
  name: NextToken
  type: string
- description: ''
  name: LastEvaluatedKey
  type: object
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-execute-statement-output-schema.json
slug: dynamodb-execute-statement-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExecuteStatementOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Items\": {\n      \"type\": \"array\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    },\n    \"LastEvaluatedKey\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-execute-statement-output-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ExecuteStatementOutput
---
