---
description: ''
layout: schema
name: UntagResourceInput
properties_list:
- description: ''
  name: ResourceArn
  type: string
- description: ''
  name: TagKeys
  type: array
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-untag-resource-input-schema.json
slug: dynamodb-untag-resource-input
source_filename: dynamodb-untag-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UntagResourceInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"type\": \"string\"\n    },\n    \"TagKeys\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-untag-resource-input-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: UntagResourceInput
---
