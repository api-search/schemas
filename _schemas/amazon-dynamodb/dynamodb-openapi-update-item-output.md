---
description: UpdateItemOutput schema from Amazon DynamoDB API
layout: schema
name: UpdateItemOutput
properties_list:
- description: A map of attribute values as they appear after the UpdateItem operation
  name: Attributes
  type: object
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-update-item-output-schema.json
slug: dynamodb-openapi-update-item-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-update-item-output-schema.json\",\n  \"title\": \"UpdateItemOutput\",\n  \"description\": \"UpdateItemOutput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Attributes\": {\n      \"type\": \"object\",\n      \"description\": \"A map of attribute values as they appear after the UpdateItem operation\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AttributeValue\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-update-item-output-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: UpdateItemOutput
---
