---
description: ''
layout: schema
name: ScanInput
properties_list:
- description: The name of the table containing the requested items
  name: TableName
  type: string
- description: The name of a secondary index to scan
  name: IndexName
  type: string
- description: A string that contains conditions that DynamoDB applies after the Scan operation, but before the data is returned
  name: FilterExpression
  type: string
- description: A string that identifies attributes to retrieve from the table
  name: ProjectionExpression
  type: string
- description: ''
  name: ExpressionAttributeNames
  type: object
- description: ''
  name: ExpressionAttributeValues
  type: object
- description: ''
  name: Select
  type: string
- description: The maximum number of items to evaluate
  name: Limit
  type: integer
- description: Whether to use strongly consistent reads
  name: ConsistentRead
  type: boolean
- description: The primary key of the first item for this scan to evaluate
  name: ExclusiveStartKey
  type: object
- description: Identifies an individual segment to be scanned by a parallel scan
  name: Segment
  type: integer
- description: Total number of segments for a parallel scan
  name: TotalSegments
  type: integer
- description: ''
  name: ReturnConsumedCapacity
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-scan-input-schema.json
slug: dynamodb-scan-input
source_filename: dynamodb-scan-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScanInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table containing the requested items\"\n    },\n    \"IndexName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of a secondary index to scan\"\n    },\n    \"FilterExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A string that contains conditions that DynamoDB applies after the Scan operation, but before the data is returned\"\n    },\n    \"ProjectionExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A string that identifies attributes to retrieve from the table\"\n    },\n    \"ExpressionAttributeNames\": {\n      \"type\": \"object\"\n    },\n    \"ExpressionAttributeValues\": {\n      \"type\": \"object\"\n    },\n    \"Select\": {\n      \"type\": \"string\"\n    },\n    \"Limit\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of items to evaluate\"\n    },\n    \"ConsistentRead\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use strongly consistent reads\"\n    },\n    \"ExclusiveStartKey\": {\n      \"type\": \"object\",\n      \"description\": \"The primary key of the first item for this scan to evaluate\"\n    },\n    \"Segment\": {\n      \"type\": \"integer\",\n      \"description\": \"Identifies an individual segment to be scanned by a parallel scan\"\n    },\n    \"TotalSegments\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of segments for a parallel scan\"\n    },\n    \"ReturnConsumedCapacity\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-scan-input-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ScanInput
---
