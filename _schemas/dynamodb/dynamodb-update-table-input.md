---
description: ''
layout: schema
name: UpdateTableInput
properties_list:
- description: The name of the table to update
  name: TableName
  type: string
- description: ''
  name: AttributeDefinitions
  type: array
- description: ''
  name: BillingMode
  type: string
- description: ''
  name: GlobalSecondaryIndexUpdates
  type: array
- description: ''
  name: TableClass
  type: string
- description: ''
  name: DeletionProtectionEnabled
  type: boolean
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-update-table-input-schema.json
slug: dynamodb-update-table-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateTableInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table to update\"\n    },\n    \"AttributeDefinitions\": {\n      \"type\": \"array\"\n    },\n    \"BillingMode\": {\n      \"type\": \"string\"\n    },\n    \"GlobalSecondaryIndexUpdates\": {\n      \"type\": \"array\"\n    },\n    \"TableClass\": {\n      \"type\": \"string\"\n    },\n    \"DeletionProtectionEnabled\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-update-table-input-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: UpdateTableInput
---
