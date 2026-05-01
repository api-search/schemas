---
description: CreateTableInput schema from Amazon DynamoDB API
layout: schema
name: CreateTableInput
properties_list:
- description: The name of the table to create
  name: TableName
  type: string
- description: Specifies the attributes that make up the primary key for the table. The attributes must also be defined in AttributeDefinitions.
  name: KeySchema
  type: array
- description: An array of attributes that describe the key schema for the table and indexes
  name: AttributeDefinitions
  type: array
- description: ''
  name: ProvisionedThroughput
  type: object
- description: Controls how you are charged for read and write throughput
  name: BillingMode
  type: string
- description: One or more global secondary indexes to be created on the table
  name: GlobalSecondaryIndexes
  type: array
- description: One or more local secondary indexes to be created on the table
  name: LocalSecondaryIndexes
  type: array
- description: Tags to associate with the table
  name: Tags
  type: array
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-create-table-input-schema.json
slug: dynamodb-openapi-create-table-input
source_filename: dynamodb-openapi-create-table-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-create-table-input-schema.json\",\n  \"title\": \"CreateTableInput\",\n  \"description\": \"CreateTableInput schema from Amazon DynamoDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table to create\",\n      \"minLength\": 3,\n      \"maxLength\": 255\n    },\n    \"KeySchema\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies the attributes that make up the primary key for the table. The attributes must also be defined in AttributeDefinitions.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KeySchemaElement\"\n      },\n      \"minItems\": 1,\n      \"maxItems\": 2\n    },\n    \"AttributeDefinitions\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"An array of attributes that describe the key schema for the table and indexes\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AttributeDefinition\"\n      }\n    },\n    \"ProvisionedThroughput\": {\n      \"$ref\": \"#/components/schemas/ProvisionedThroughput\"\n    },\n    \"BillingMode\": {\n      \"type\": \"string\",\n      \"description\": \"Controls how you are charged for read and write throughput\",\n      \"enum\": [\n        \"PROVISIONED\",\n        \"PAY_PER_REQUEST\"\n      ]\n    },\n    \"GlobalSecondaryIndexes\": {\n      \"type\": \"array\",\n      \"description\": \"One or more global secondary indexes to be created on the table\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/GlobalSecondaryIndex\"\n      }\n    },\n    \"LocalSecondaryIndexes\": {\n      \"type\": \"array\",\n      \"description\": \"One or more local secondary indexes to be created on the table\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LocalSecondaryIndex\"\
  \n      }\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags to associate with the table\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    }\n  },\n  \"required\": [\n    \"TableName\",\n    \"KeySchema\",\n    \"AttributeDefinitions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-create-table-input-schema.json
tags:
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: CreateTableInput
---
