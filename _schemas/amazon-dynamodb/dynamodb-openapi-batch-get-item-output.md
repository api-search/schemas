---
description: BatchGetItemOutput schema from Amazon DynamoDB API
layout: schema
name: BatchGetItemOutput
properties_list:
- description: A map of table names to lists of items retrieved
  name: Responses
  type: object
- description: A map of unprocessed keys, to be retried
  name: UnprocessedKeys
  type: object
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-batch-get-item-output-schema.json
slug: dynamodb-openapi-batch-get-item-output
source_filename: dynamodb-openapi-batch-get-item-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-batch-get-item-output-schema.json\",\n  \"title\": \"BatchGetItemOutput\",\n  \"description\": \"BatchGetItemOutput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Responses\": {\n      \"type\": \"object\",\n      \"description\": \"A map of table names to lists of items retrieved\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/components/schemas/AttributeValue\"\n          }\n        }\n      }\n    },\n    \"UnprocessedKeys\": {\n      \"type\": \"object\",\n      \"description\": \"A map of unprocessed keys, to be retried\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-batch-get-item-output-schema.json
tags:
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: BatchGetItemOutput
---
