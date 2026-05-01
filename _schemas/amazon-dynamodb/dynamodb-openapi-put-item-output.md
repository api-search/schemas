---
description: PutItemOutput schema from Amazon DynamoDB API
layout: schema
name: PutItemOutput
properties_list:
- description: The attribute values as they appeared before the PutItem operation
  name: Attributes
  type: object
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-put-item-output-schema.json
slug: dynamodb-openapi-put-item-output
source_filename: dynamodb-openapi-put-item-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-put-item-output-schema.json\",\n  \"title\": \"PutItemOutput\",\n  \"description\": \"PutItemOutput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Attributes\": {\n      \"type\": \"object\",\n      \"description\": \"The attribute values as they appeared before the PutItem operation\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AttributeValue\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-put-item-output-schema.json
tags:
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: PutItemOutput
---
