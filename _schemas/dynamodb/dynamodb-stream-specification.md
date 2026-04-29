---
description: ''
layout: schema
name: StreamSpecification
properties_list:
- description: Indicates whether DynamoDB Streams is enabled on the table
  name: StreamEnabled
  type: boolean
- description: Determines the information written to the stream for this table
  name: StreamViewType
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-stream-specification-schema.json
slug: dynamodb-stream-specification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StreamSpecification\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StreamEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether DynamoDB Streams is enabled on the table\"\n    },\n    \"StreamViewType\": {\n      \"type\": \"string\",\n      \"description\": \"Determines the information written to the stream for this table\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-stream-specification-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: StreamSpecification
---
