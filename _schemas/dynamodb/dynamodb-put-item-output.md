---
description: ''
layout: schema
name: PutItemOutput
properties_list:
- description: The attribute values as they appeared before the PutItem operation
  name: Attributes
  type: object
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-put-item-output-schema.json
slug: dynamodb-put-item-output
source_filename: dynamodb-put-item-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PutItemOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Attributes\": {\n      \"type\": \"object\",\n      \"description\": \"The attribute values as they appeared before the PutItem operation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-put-item-output-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: PutItemOutput
---
