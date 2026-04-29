---
description: UpdateTableInput schema from Amazon DynamoDB API
layout: schema
name: UpdateTableInput
properties_list:
- description: The name of the table to update
  name: TableName
  type: string
- description: ''
  name: ProvisionedThroughput
  type: object
- description: ''
  name: BillingMode
  type: string
- description: An array of global secondary index operations
  name: GlobalSecondaryIndexUpdates
  type: array
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-update-table-input-schema.json
slug: dynamodb-openapi-update-table-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-update-table-input-schema.json\",\n  \"title\": \"UpdateTableInput\",\n  \"description\": \"UpdateTableInput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table to update\"\n    },\n    \"ProvisionedThroughput\": {\n      \"$ref\": \"#/components/schemas/ProvisionedThroughput\"\n    },\n    \"BillingMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PROVISIONED\",\n        \"PAY_PER_REQUEST\"\n      ]\n    },\n    \"GlobalSecondaryIndexUpdates\": {\n      \"type\": \"array\",\n      \"description\": \"An array of global secondary index operations\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"required\": [\n \
  \   \"TableName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-update-table-input-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: UpdateTableInput
---
