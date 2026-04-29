---
description: ''
layout: schema
name: QueryInput
properties_list:
- description: The name of the table containing the requested items
  name: TableName
  type: string
- description: The name of a secondary index to query
  name: IndexName
  type: string
- description: The condition that specifies the key values for items to be retrieved by the Query action. Must specify the partition key name and value as an equality condition.
  name: KeyConditionExpression
  type: string
- description: A string that contains conditions that DynamoDB applies after the Query operation, but before the data is returned
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
- description: The attributes to be returned in the result
  name: Select
  type: string
- description: If true (default), the traversal is performed in ascending order; if false, in descending order
  name: ScanIndexForward
  type: boolean
- description: The maximum number of items to evaluate
  name: Limit
  type: integer
- description: Whether to use strongly consistent reads
  name: ConsistentRead
  type: boolean
- description: The primary key of the first item for this query to evaluate
  name: ExclusiveStartKey
  type: object
- description: ''
  name: ReturnConsumedCapacity
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-query-input-schema.json
slug: dynamodb-query-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table containing the requested items\"\n    },\n    \"IndexName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of a secondary index to query\"\n    },\n    \"KeyConditionExpression\": {\n      \"type\": \"string\",\n      \"description\": \"The condition that specifies the key values for items to be retrieved by the Query action. Must specify the partition key name and value as an equality condition.\"\n    },\n    \"FilterExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A string that contains conditions that DynamoDB applies after the Query operation, but before the data is returned\"\n    },\n    \"ProjectionExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A string that identifies\
  \ attributes to retrieve from the table\"\n    },\n    \"ExpressionAttributeNames\": {\n      \"type\": \"object\"\n    },\n    \"ExpressionAttributeValues\": {\n      \"type\": \"object\"\n    },\n    \"Select\": {\n      \"type\": \"string\",\n      \"description\": \"The attributes to be returned in the result\"\n    },\n    \"ScanIndexForward\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true (default), the traversal is performed in ascending order; if false, in descending order\"\n    },\n    \"Limit\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of items to evaluate\"\n    },\n    \"ConsistentRead\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use strongly consistent reads\"\n    },\n    \"ExclusiveStartKey\": {\n      \"type\": \"object\",\n      \"description\": \"The primary key of the first item for this query to evaluate\"\n    },\n    \"ReturnConsumedCapacity\": {\n      \"type\": \"string\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-query-input-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: QueryInput
---
