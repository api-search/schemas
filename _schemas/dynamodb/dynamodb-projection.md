---
description: ''
layout: schema
name: Projection
properties_list:
- description: The set of attributes that are projected into the index
  name: ProjectionType
  type: string
- description: List of non-key attribute names that are projected into the index
  name: NonKeyAttributes
  type: array
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-projection-schema.json
slug: dynamodb-projection
source_filename: dynamodb-projection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Projection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProjectionType\": {\n      \"type\": \"string\",\n      \"description\": \"The set of attributes that are projected into the index\"\n    },\n    \"NonKeyAttributes\": {\n      \"type\": \"array\",\n      \"description\": \"List of non-key attribute names that are projected into the index\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-projection-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: Projection
---
