---
description: ''
layout: schema
name: ScanOutput
properties_list:
- description: An array of item attributes that match the scan criteria
  name: Items
  type: array
- description: The number of items in the response
  name: Count
  type: integer
- description: The number of items evaluated before any filter was applied
  name: ScannedCount
  type: integer
- description: The primary key of the item where the operation stopped. Use this value for ExclusiveStartKey in a new request to continue the scan.
  name: LastEvaluatedKey
  type: object
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-scan-output-schema.json
slug: dynamodb-scan-output
source_filename: dynamodb-scan-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScanOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Items\": {\n      \"type\": \"array\",\n      \"description\": \"An array of item attributes that match the scan criteria\"\n    },\n    \"Count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items in the response\"\n    },\n    \"ScannedCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items evaluated before any filter was applied\"\n    },\n    \"LastEvaluatedKey\": {\n      \"type\": \"object\",\n      \"description\": \"The primary key of the item where the operation stopped. Use this value for ExclusiveStartKey in a new request to continue the scan.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-scan-output-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ScanOutput
---
