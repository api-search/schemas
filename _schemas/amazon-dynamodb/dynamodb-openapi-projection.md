---
description: Represents attributes that are copied from the table into an index
layout: schema
name: Projection
properties_list:
- description: The set of attributes that are projected into the index
  name: ProjectionType
  type: string
- description: The non-key projected attributes
  name: NonKeyAttributes
  type: array
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-projection-schema.json
slug: dynamodb-openapi-projection
source_filename: dynamodb-openapi-projection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-projection-schema.json\",\n  \"title\": \"Projection\",\n  \"description\": \"Represents attributes that are copied from the table into an index\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProjectionType\": {\n      \"type\": \"string\",\n      \"description\": \"The set of attributes that are projected into the index\",\n      \"enum\": [\n        \"ALL\",\n        \"KEYS_ONLY\",\n        \"INCLUDE\"\n      ]\n    },\n    \"NonKeyAttributes\": {\n      \"type\": \"array\",\n      \"description\": \"The non-key projected attributes\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"maxItems\": 20\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-projection-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: Projection
---
