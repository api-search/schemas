---
description: ''
layout: schema
name: GetItemOutput
properties_list:
- description: A map of attribute names to AttributeValue objects. Only returned if the item with the given primary key exists.
  name: Item
  type: object
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-get-item-output-schema.json
slug: dynamodb-get-item-output
source_filename: dynamodb-get-item-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetItemOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Item\": {\n      \"type\": \"object\",\n      \"description\": \"A map of attribute names to AttributeValue objects. Only returned if the item with the given primary key exists.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-get-item-output-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: GetItemOutput
---
