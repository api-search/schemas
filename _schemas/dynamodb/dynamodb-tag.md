---
description: ''
layout: schema
name: Tag
properties_list:
- description: The key of the tag
  name: Key
  type: string
- description: The value of the tag
  name: Value
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-tag-schema.json
slug: dynamodb-tag
source_filename: dynamodb-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tag\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the tag\"\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the tag\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-tag-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: Tag
---
