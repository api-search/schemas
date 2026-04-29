---
description: ''
layout: schema
name: QueryOutput
properties_list:
- description: An array of item attributes that match the query criteria
  name: Items
  type: array
- description: The number of items in the response
  name: Count
  type: integer
- description: The number of items evaluated before any filter was applied
  name: ScannedCount
  type: integer
- description: The primary key of the item where the operation stopped, inclusive of the previous result set. Use this value for ExclusiveStartKey in a new request to continue the query.
  name: LastEvaluatedKey
  type: object
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-query-output-schema.json
slug: dynamodb-query-output
source_filename: dynamodb-query-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Items\": {\n      \"type\": \"array\",\n      \"description\": \"An array of item attributes that match the query criteria\"\n    },\n    \"Count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items in the response\"\n    },\n    \"ScannedCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items evaluated before any filter was applied\"\n    },\n    \"LastEvaluatedKey\": {\n      \"type\": \"object\",\n      \"description\": \"The primary key of the item where the operation stopped, inclusive of the previous result set. Use this value for ExclusiveStartKey in a new request to continue the query.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-query-output-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: QueryOutput
---
