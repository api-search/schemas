---
description: ''
layout: schema
name: ImportTableInput
properties_list:
- description: Idempotency token
  name: ClientToken
  type: string
- description: ''
  name: S3BucketSource
  type: object
- description: ''
  name: InputFormat
  type: string
- description: ''
  name: InputFormatOptions
  type: object
- description: ''
  name: InputCompressionType
  type: string
- description: ''
  name: TableCreationParameters
  type: object
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-import-table-input-schema.json
slug: dynamodb-import-table-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImportTableInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientToken\": {\n      \"type\": \"string\",\n      \"description\": \"Idempotency token\"\n    },\n    \"S3BucketSource\": {\n      \"type\": \"object\"\n    },\n    \"InputFormat\": {\n      \"type\": \"string\"\n    },\n    \"InputFormatOptions\": {\n      \"type\": \"object\"\n    },\n    \"InputCompressionType\": {\n      \"type\": \"string\"\n    },\n    \"TableCreationParameters\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-import-table-input-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ImportTableInput
---
