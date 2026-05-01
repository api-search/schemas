---
description: Represents the properties of a global secondary index
layout: schema
name: GlobalSecondaryIndex
properties_list:
- description: The name of the global secondary index
  name: IndexName
  type: string
- description: The complete key schema for the index
  name: KeySchema
  type: array
- description: ''
  name: Projection
  type: object
- description: ''
  name: ProvisionedThroughput
  type: object
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-global-secondary-index-schema.json
slug: dynamodb-openapi-global-secondary-index
source_filename: dynamodb-openapi-global-secondary-index-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-global-secondary-index-schema.json\",\n  \"title\": \"GlobalSecondaryIndex\",\n  \"description\": \"Represents the properties of a global secondary index\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IndexName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the global secondary index\"\n    },\n    \"KeySchema\": {\n      \"type\": \"array\",\n      \"description\": \"The complete key schema for the index\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KeySchemaElement\"\n      },\n      \"minItems\": 1,\n      \"maxItems\": 2\n    },\n    \"Projection\": {\n      \"$ref\": \"#/components/schemas/Projection\"\n    },\n    \"ProvisionedThroughput\": {\n      \"$ref\": \"#/components/schemas/ProvisionedThroughput\"\n    }\n  },\n  \"required\"\
  : [\n    \"IndexName\",\n    \"KeySchema\",\n    \"Projection\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-global-secondary-index-schema.json
tags:
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: GlobalSecondaryIndex
---
