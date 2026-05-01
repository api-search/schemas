---
description: ''
layout: schema
name: KeySchemaElement
properties_list:
- description: The name of a key attribute
  name: AttributeName
  type: string
- description: 'The role of the key attribute: HASH (partition key) or RANGE (sort key)'
  name: KeyType
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-key-schema-element-schema.json
slug: dynamodb-key-schema-element
source_filename: dynamodb-key-schema-element-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeySchemaElement\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AttributeName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of a key attribute\"\n    },\n    \"KeyType\": {\n      \"type\": \"string\",\n      \"description\": \"The role of the key attribute: HASH (partition key) or RANGE (sort key)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-key-schema-element-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: KeySchemaElement
---
