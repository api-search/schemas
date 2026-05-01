---
description: ''
layout: schema
name: TagResourceInput
properties_list:
- description: ARN of the DynamoDB resource to tag
  name: ResourceArn
  type: string
- description: Tags to associate with the resource
  name: Tags
  type: array
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-tag-resource-input-schema.json
slug: dynamodb-tag-resource-input
source_filename: dynamodb-tag-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagResourceInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the DynamoDB resource to tag\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags to associate with the resource\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-tag-resource-input-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: TagResourceInput
---
