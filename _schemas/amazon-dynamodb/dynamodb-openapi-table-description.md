---
description: Represents the properties of a DynamoDB table
layout: schema
name: TableDescription
properties_list:
- description: The name of the table
  name: TableName
  type: string
- description: The current state of the table
  name: TableStatus
  type: string
- description: The Amazon Resource Name (ARN) of the table
  name: TableArn
  type: string
- description: Unique identifier for the table
  name: TableId
  type: string
- description: The date and time when the table was created
  name: CreationDateTime
  type: number
- description: The primary key structure for the table
  name: KeySchema
  type: array
- description: An array of attribute definitions for the table
  name: AttributeDefinitions
  type: array
- description: ''
  name: ProvisionedThroughput
  type: object
- description: The total size of the table in bytes
  name: TableSizeBytes
  type: integer
- description: The number of items in the table
  name: ItemCount
  type: integer
- description: The global secondary indexes on the table
  name: GlobalSecondaryIndexes
  type: array
- description: The local secondary indexes on the table
  name: LocalSecondaryIndexes
  type: array
- description: Contains details about the billing mode for the table
  name: BillingModeSummary
  type: object
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-table-description-schema.json
slug: dynamodb-openapi-table-description
source_filename: dynamodb-openapi-table-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-table-description-schema.json\",\n  \"title\": \"TableDescription\",\n  \"description\": \"Represents the properties of a DynamoDB table\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table\"\n    },\n    \"TableStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the table\",\n      \"enum\": [\n        \"CREATING\",\n        \"UPDATING\",\n        \"DELETING\",\n        \"ACTIVE\",\n        \"INACCESSIBLE_ENCRYPTION_CREDENTIALS\",\n        \"ARCHIVING\",\n        \"ARCHIVED\"\n      ]\n    },\n    \"TableArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the table\"\n    },\n    \"TableId\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Unique identifier for the table\"\n    },\n    \"CreationDateTime\": {\n      \"type\": \"number\",\n      \"description\": \"The date and time when the table was created\"\n    },\n    \"KeySchema\": {\n      \"type\": \"array\",\n      \"description\": \"The primary key structure for the table\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KeySchemaElement\"\n      }\n    },\n    \"AttributeDefinitions\": {\n      \"type\": \"array\",\n      \"description\": \"An array of attribute definitions for the table\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AttributeDefinition\"\n      }\n    },\n    \"ProvisionedThroughput\": {\n      \"$ref\": \"#/components/schemas/ProvisionedThroughputDescription\"\n    },\n    \"TableSizeBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"The total size of the table in bytes\"\n    },\n    \"ItemCount\": {\n      \"type\": \"integer\",\n      \"description\":\
  \ \"The number of items in the table\"\n    },\n    \"GlobalSecondaryIndexes\": {\n      \"type\": \"array\",\n      \"description\": \"The global secondary indexes on the table\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"LocalSecondaryIndexes\": {\n      \"type\": \"array\",\n      \"description\": \"The local secondary indexes on the table\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"BillingModeSummary\": {\n      \"type\": \"object\",\n      \"description\": \"Contains details about the billing mode for the table\",\n      \"properties\": {\n        \"BillingMode\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"PROVISIONED\",\n            \"PAY_PER_REQUEST\"\n          ]\n        },\n        \"LastUpdateToPayPerRequestDateTime\": {\n          \"type\": \"number\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-table-description-schema.json
tags:
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: TableDescription
---
