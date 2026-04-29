---
description: Request body for updating a function's configuration
layout: schema
name: UpdateFunctionConfigurationRequest
properties_list:
- description: The ARN of the function's execution role
  name: Role
  type: string
- description: The name of the function handler
  name: Handler
  type: string
- description: A description of the function
  name: Description
  type: string
- description: Execution timeout in seconds
  name: Timeout
  type: integer
- description: Memory allocated in MB
  name: MemorySize
  type: integer
- description: ''
  name: Environment
  type: object
- description: The runtime identifier
  name: Runtime
  type: string
- description: ''
  name: DeadLetterConfig
  type: object
- description: ''
  name: KMSKeyArn
  type: string
- description: ''
  name: TracingConfig
  type: object
- description: Update only if the revision ID matches. Prevents modifying a function that has changed since you last read it.
  name: RevisionId
  type: string
- description: ''
  name: Layers
  type: array
- description: ''
  name: EphemeralStorage
  type: object
- description: ''
  name: SnapStart
  type: object
- description: ''
  name: LoggingConfig
  type: object
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-update-function-configuration-request-schema.json
slug: aws-lambda-update-function-configuration-request
source_filename: aws-lambda-update-function-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateFunctionConfigurationRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a function's configuration\",\n  \"properties\": {\n    \"Role\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the function's execution role\"\n    },\n    \"Handler\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the function handler\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the function\"\n    },\n    \"Timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Execution timeout in seconds\"\n    },\n    \"MemorySize\": {\n      \"type\": \"integer\",\n      \"description\": \"Memory allocated in MB\"\n    },\n    \"Environment\": {\n      \"type\": \"object\"\n    },\n    \"Runtime\": {\n      \"type\": \"string\",\n      \"description\": \"The runtime identifier\"\
  \n    },\n    \"DeadLetterConfig\": {\n      \"type\": \"object\"\n    },\n    \"KMSKeyArn\": {\n      \"type\": \"string\"\n    },\n    \"TracingConfig\": {\n      \"type\": \"object\"\n    },\n    \"RevisionId\": {\n      \"type\": \"string\",\n      \"description\": \"Update only if the revision ID matches. Prevents modifying a function that has changed since you last read it.\"\n    },\n    \"Layers\": {\n      \"type\": \"array\"\n    },\n    \"EphemeralStorage\": {\n      \"type\": \"object\"\n    },\n    \"SnapStart\": {\n      \"type\": \"object\"\n    },\n    \"LoggingConfig\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-update-function-configuration-request-schema.json
tags: []
title: UpdateFunctionConfigurationRequest
---
