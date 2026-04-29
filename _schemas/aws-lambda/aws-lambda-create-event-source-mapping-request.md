---
description: Request body for creating an event source mapping
layout: schema
name: CreateEventSourceMappingRequest
properties_list:
- description: The ARN of the event source. Required for Kinesis, DynamoDB Streams, SQS, MQ, MSK, and DocumentDB.
  name: EventSourceArn
  type: string
- description: The name or ARN of the Lambda function
  name: FunctionName
  type: string
- description: If true, the event source mapping is active
  name: Enabled
  type: boolean
- description: Maximum number of records in each batch
  name: BatchSize
  type: integer
- description: Maximum time to gather records before invoking
  name: MaximumBatchingWindowInSeconds
  type: integer
- description: Number of batches to process concurrently per shard
  name: ParallelizationFactor
  type: integer
- description: Starting position in the stream
  name: StartingPosition
  type: string
- description: ''
  name: StartingPositionTimestamp
  type: string
- description: ''
  name: MaximumRecordAgeInSeconds
  type: integer
- description: ''
  name: BisectBatchOnFunctionError
  type: boolean
- description: ''
  name: MaximumRetryAttempts
  type: integer
- description: ''
  name: TumblingWindowInSeconds
  type: integer
- description: ''
  name: FunctionResponseTypes
  type: array
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-create-event-source-mapping-request-schema.json
slug: aws-lambda-create-event-source-mapping-request
source_filename: aws-lambda-create-event-source-mapping-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateEventSourceMappingRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating an event source mapping\",\n  \"properties\": {\n    \"EventSourceArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the event source. Required for Kinesis, DynamoDB Streams, SQS, MQ, MSK, and DocumentDB.\"\n    },\n    \"FunctionName\": {\n      \"type\": \"string\",\n      \"description\": \"The name or ARN of the Lambda function\"\n    },\n    \"Enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the event source mapping is active\"\n    },\n    \"BatchSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of records in each batch\"\n    },\n    \"MaximumBatchingWindowInSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum time to gather records before invoking\"\n    },\n    \"ParallelizationFactor\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Number of batches to process concurrently per shard\"\n    },\n    \"StartingPosition\": {\n      \"type\": \"string\",\n      \"description\": \"Starting position in the stream\"\n    },\n    \"StartingPositionTimestamp\": {\n      \"type\": \"string\"\n    },\n    \"MaximumRecordAgeInSeconds\": {\n      \"type\": \"integer\"\n    },\n    \"BisectBatchOnFunctionError\": {\n      \"type\": \"boolean\"\n    },\n    \"MaximumRetryAttempts\": {\n      \"type\": \"integer\"\n    },\n    \"TumblingWindowInSeconds\": {\n      \"type\": \"integer\"\n    },\n    \"FunctionResponseTypes\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-create-event-source-mapping-request-schema.json
tags: []
title: CreateEventSourceMappingRequest
---
