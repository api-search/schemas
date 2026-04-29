---
description: Request body for updating an event source mapping
layout: schema
name: UpdateEventSourceMappingRequest
properties_list:
- description: The name or ARN of the Lambda function
  name: FunctionName
  type: string
- description: If true, the event source mapping is active
  name: Enabled
  type: boolean
- description: ''
  name: BatchSize
  type: integer
- description: ''
  name: MaximumBatchingWindowInSeconds
  type: integer
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
  name: ParallelizationFactor
  type: integer
- description: ''
  name: TumblingWindowInSeconds
  type: integer
- description: ''
  name: FunctionResponseTypes
  type: array
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-update-event-source-mapping-request-schema.json
slug: aws-lambda-update-event-source-mapping-request
source_filename: aws-lambda-update-event-source-mapping-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateEventSourceMappingRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating an event source mapping\",\n  \"properties\": {\n    \"FunctionName\": {\n      \"type\": \"string\",\n      \"description\": \"The name or ARN of the Lambda function\"\n    },\n    \"Enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the event source mapping is active\"\n    },\n    \"BatchSize\": {\n      \"type\": \"integer\"\n    },\n    \"MaximumBatchingWindowInSeconds\": {\n      \"type\": \"integer\"\n    },\n    \"MaximumRecordAgeInSeconds\": {\n      \"type\": \"integer\"\n    },\n    \"BisectBatchOnFunctionError\": {\n      \"type\": \"boolean\"\n    },\n    \"MaximumRetryAttempts\": {\n      \"type\": \"integer\"\n    },\n    \"ParallelizationFactor\": {\n      \"type\": \"integer\"\n    },\n    \"TumblingWindowInSeconds\": {\n      \"type\": \"integer\"\
  \n    },\n    \"FunctionResponseTypes\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-update-event-source-mapping-request-schema.json
tags: []
title: UpdateEventSourceMappingRequest
---
