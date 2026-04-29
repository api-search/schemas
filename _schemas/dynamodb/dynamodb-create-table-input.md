---
description: ''
layout: schema
name: CreateTableInput
properties_list:
- description: The name of the table to create. Must be between 3 and 255 characters long.
  name: TableName
  type: string
- description: An array of attributes that describe the key schema for the table and indexes
  name: AttributeDefinitions
  type: array
- description: Specifies the attributes that make up the primary key for a table or an index
  name: KeySchema
  type: array
- description: Controls how you are charged for read and write throughput
  name: BillingMode
  type: string
- description: One or more global secondary indexes to create on the table
  name: GlobalSecondaryIndexes
  type: array
- description: One or more local secondary indexes to create on the table
  name: LocalSecondaryIndexes
  type: array
- description: Tags to associate with the table
  name: Tags
  type: array
- description: The table class of the new table
  name: TableClass
  type: string
- description: Indicates whether deletion protection is enabled
  name: DeletionProtectionEnabled
  type: boolean
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-create-table-input-schema.json
slug: dynamodb-create-table-input
source_filename: dynamodb-create-table-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateTableInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table to create. Must be between 3 and 255 characters long.\"\n    },\n    \"AttributeDefinitions\": {\n      \"type\": \"array\",\n      \"description\": \"An array of attributes that describe the key schema for the table and indexes\"\n    },\n    \"KeySchema\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies the attributes that make up the primary key for a table or an index\"\n    },\n    \"BillingMode\": {\n      \"type\": \"string\",\n      \"description\": \"Controls how you are charged for read and write throughput\"\n    },\n    \"GlobalSecondaryIndexes\": {\n      \"type\": \"array\",\n      \"description\": \"One or more global secondary indexes to create on the table\"\n    },\n    \"LocalSecondaryIndexes\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"One or more local secondary indexes to create on the table\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags to associate with the table\"\n    },\n    \"TableClass\": {\n      \"type\": \"string\",\n      \"description\": \"The table class of the new table\"\n    },\n    \"DeletionProtectionEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether deletion protection is enabled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-create-table-input-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: CreateTableInput
---
