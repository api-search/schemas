---
description: QueryOutput schema from Amazon DynamoDB API
layout: schema
name: QueryOutput
properties_list:
- description: An array of item attributes that match the query criteria
  name: Items
  type: array
- description: The number of items in the response
  name: Count
  type: integer
- description: The number of items evaluated before any filter is applied
  name: ScannedCount
  type: integer
- description: The primary key of the item where the operation stopped
  name: LastEvaluatedKey
  type: object
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-query-output-schema.json
slug: dynamodb-openapi-query-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-query-output-schema.json\",\n  \"title\": \"QueryOutput\",\n  \"description\": \"QueryOutput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Items\": {\n      \"type\": \"array\",\n      \"description\": \"An array of item attributes that match the query criteria\",\n      \"items\": {\n        \"type\": \"object\",\n        \"additionalProperties\": {\n          \"$ref\": \"#/components/schemas/AttributeValue\"\n        }\n      }\n    },\n    \"Count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items in the response\"\n    },\n    \"ScannedCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items evaluated before any filter is applied\"\n    },\n    \"LastEvaluatedKey\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"The primary key of the item where the operation stopped\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AttributeValue\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-query-output-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: QueryOutput
---
