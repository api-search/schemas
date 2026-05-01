---
description: Represents the properties of a local secondary index
layout: schema
name: LocalSecondaryIndex
properties_list:
- description: The name of the local secondary index
  name: IndexName
  type: string
- description: The complete key schema for the index
  name: KeySchema
  type: array
- description: ''
  name: Projection
  type: object
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-local-secondary-index-schema.json
slug: dynamodb-openapi-local-secondary-index
source_filename: dynamodb-openapi-local-secondary-index-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-local-secondary-index-schema.json\",\n  \"title\": \"LocalSecondaryIndex\",\n  \"description\": \"Represents the properties of a local secondary index\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IndexName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the local secondary index\"\n    },\n    \"KeySchema\": {\n      \"type\": \"array\",\n      \"description\": \"The complete key schema for the index\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KeySchemaElement\"\n      },\n      \"minItems\": 2,\n      \"maxItems\": 2\n    },\n    \"Projection\": {\n      \"$ref\": \"#/components/schemas/Projection\"\n    }\n  },\n  \"required\": [\n    \"IndexName\",\n    \"KeySchema\",\n    \"Projection\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-local-secondary-index-schema.json
tags:
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: LocalSecondaryIndex
---
