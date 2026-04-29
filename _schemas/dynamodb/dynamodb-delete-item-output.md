---
description: ''
layout: schema
name: DeleteItemOutput
properties_list:
- description: The attribute values as they appeared before the item was deleted
  name: Attributes
  type: object
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-delete-item-output-schema.json
slug: dynamodb-delete-item-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteItemOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Attributes\": {\n      \"type\": \"object\",\n      \"description\": \"The attribute values as they appeared before the item was deleted\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-delete-item-output-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: DeleteItemOutput
---
