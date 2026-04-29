---
description: Tag schema from Amazon DynamoDB API
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
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-tag-schema.json
slug: dynamodb-openapi-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"Tag schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the tag\",\n      \"minLength\": 1,\n      \"maxLength\": 128\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the tag\",\n      \"minLength\": 0,\n      \"maxLength\": 256\n    }\n  },\n  \"required\": [\n    \"Key\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-tag-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: Tag
---
