---
description: Represents a single element of a key schema
layout: schema
name: KeySchemaElement
properties_list:
- description: The name of a key attribute
  name: AttributeName
  type: string
- description: The role that this key attribute will assume
  name: KeyType
  type: string
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-key-schema-element-schema.json
slug: dynamodb-openapi-key-schema-element
source_filename: dynamodb-openapi-key-schema-element-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-key-schema-element-schema.json\",\n  \"title\": \"KeySchemaElement\",\n  \"description\": \"Represents a single element of a key schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AttributeName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of a key attribute\"\n    },\n    \"KeyType\": {\n      \"type\": \"string\",\n      \"description\": \"The role that this key attribute will assume\",\n      \"enum\": [\n        \"HASH\",\n        \"RANGE\"\n      ]\n    }\n  },\n  \"required\": [\n    \"AttributeName\",\n    \"KeyType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-key-schema-element-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: KeySchemaElement
---
