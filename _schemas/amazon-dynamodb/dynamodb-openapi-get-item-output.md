---
description: GetItemOutput schema from Amazon DynamoDB API
layout: schema
name: GetItemOutput
properties_list:
- description: A map of attribute names to AttributeValue objects
  name: Item
  type: object
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-get-item-output-schema.json
slug: dynamodb-openapi-get-item-output
source_filename: dynamodb-openapi-get-item-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-get-item-output-schema.json\",\n  \"title\": \"GetItemOutput\",\n  \"description\": \"GetItemOutput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Item\": {\n      \"type\": \"object\",\n      \"description\": \"A map of attribute names to AttributeValue objects\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AttributeValue\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-get-item-output-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: GetItemOutput
---
