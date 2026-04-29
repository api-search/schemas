---
description: Request body for creating a Lambda function
layout: schema
name: CreateFunctionRequest
properties_list:
- description: The name of the Lambda function (1-64 characters). Can also specify an ARN.
  name: FunctionName
  type: string
- description: The identifier of the function's runtime. Required for .zip file deployment packages.
  name: Runtime
  type: string
- description: The ARN of the function's execution role
  name: Role
  type: string
- description: The name of the function handler (e.g. index.handler)
  name: Handler
  type: string
- description: Description of the function
  name: Description
  type: string
- description: Execution timeout in seconds
  name: Timeout
  type: integer
- description: Memory allocated in MB
  name: MemorySize
  type: integer
- description: Set to true to publish the first version of the function
  name: Publish
  type: boolean
- description: The type of deployment package
  name: PackageType
  type: string
- description: ''
  name: DeadLetterConfig
  type: object
- description: ''
  name: Environment
  type: object
- description: ARN of the KMS key to encrypt environment variables
  name: KMSKeyArn
  type: string
- description: ''
  name: TracingConfig
  type: object
- description: Key-value pairs for tagging the function
  name: Tags
  type: object
- description: A list of function layer ARNs (with version) to add to the function's execution environment. Up to five layers.
  name: Layers
  type: array
- description: The instruction set architecture
  name: Architectures
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
schema_file: json-schema/aws-lambda-create-function-request-schema.json
slug: aws-lambda-create-function-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateFunctionRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a Lambda function\",\n  \"properties\": {\n    \"FunctionName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Lambda function (1-64 characters). Can also specify an ARN.\"\n    },\n    \"Runtime\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the function's runtime. Required for .zip file deployment packages.\"\n    },\n    \"Role\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the function's execution role\"\n    },\n    \"Handler\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the function handler (e.g. index.handler)\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the function\"\n    },\n    \"Timeout\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Execution timeout in seconds\"\n    },\n    \"MemorySize\": {\n      \"type\": \"integer\",\n      \"description\": \"Memory allocated in MB\"\n    },\n    \"Publish\": {\n      \"type\": \"boolean\",\n      \"description\": \"Set to true to publish the first version of the function\"\n    },\n    \"PackageType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of deployment package\"\n    },\n    \"DeadLetterConfig\": {\n      \"type\": \"object\"\n    },\n    \"Environment\": {\n      \"type\": \"object\"\n    },\n    \"KMSKeyArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the KMS key to encrypt environment variables\"\n    },\n    \"TracingConfig\": {\n      \"type\": \"object\"\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs for tagging the function\"\n    },\n    \"Layers\": {\n      \"type\": \"array\",\n      \"description\": \"A list of function layer ARNs (with\
  \ version) to add to the function's execution environment. Up to five layers.\"\n    },\n    \"Architectures\": {\n      \"type\": \"array\",\n      \"description\": \"The instruction set architecture\"\n    },\n    \"EphemeralStorage\": {\n      \"type\": \"object\"\n    },\n    \"SnapStart\": {\n      \"type\": \"object\"\n    },\n    \"LoggingConfig\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-create-function-request-schema.json
tags: []
title: CreateFunctionRequest
---
