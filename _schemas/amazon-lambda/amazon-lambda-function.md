---
description: An AWS Lambda function.
layout: schema
name: Function
properties_list:
- description: The name of the function.
  name: FunctionName
  type: string
- description: The function's Amazon Resource Name (ARN).
  name: FunctionArn
  type: string
- description: The function's runtime identifier.
  name: Runtime
  type: string
- description: The function's execution role ARN.
  name: Role
  type: string
- description: The function that Lambda calls to begin execution.
  name: Handler
  type: string
- description: The size of the function's deployment package, in bytes.
  name: CodeSize
  type: integer
- description: The function's description.
  name: Description
  type: string
- description: The amount of time (in seconds) that Lambda allows a function to run.
  name: Timeout
  type: integer
- description: The amount of memory available to the function at runtime.
  name: MemorySize
  type: integer
- description: The date and time the function was last updated.
  name: LastModified
  type: string
- description: The current state of the function.
  name: State
  type: string
- description: The type of deployment package.
  name: PackageType
  type: string
provider_name: Amazon Lambda
provider_slug: amazon-lambda
schema_file: json-schema/amazon-lambda-function-schema.json
slug: amazon-lambda-function
source_filename: amazon-lambda-function-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lambda/refs/heads/main/json-schema/amazon-lambda-function-schema.json\",\n  \"title\": \"Function\",\n  \"description\": \"An AWS Lambda function.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FunctionName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the function.\",\n      \"example\": \"my-function\"\n    },\n    \"FunctionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The function's Amazon Resource Name (ARN).\"\n    },\n    \"Runtime\": {\n      \"type\": \"string\",\n      \"description\": \"The function's runtime identifier.\",\n      \"example\": \"python3.12\",\n      \"enum\": [\n        \"nodejs20.x\",\n        \"python3.12\",\n        \"java21\",\n        \"go1.x\",\n        \"ruby3.2\",\n        \"dotnet8\",\n        \"provided.al2023\"\n      ]\n    },\n    \"Role\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"The function's execution role ARN.\"\n    },\n    \"Handler\": {\n      \"type\": \"string\",\n      \"description\": \"The function that Lambda calls to begin execution.\",\n      \"example\": \"lambda_function.lambda_handler\"\n    },\n    \"CodeSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the function's deployment package, in bytes.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The function's description.\"\n    },\n    \"Timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of time (in seconds) that Lambda allows a function to run.\",\n      \"example\": 30\n    },\n    \"MemorySize\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of memory available to the function at runtime.\",\n      \"example\": 128\n    },\n    \"LastModified\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time\
  \ the function was last updated.\",\n      \"format\": \"date-time\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the function.\",\n      \"example\": \"Active\",\n      \"enum\": [\n        \"Pending\",\n        \"Active\",\n        \"Inactive\",\n        \"Failed\"\n      ]\n    },\n    \"PackageType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of deployment package.\",\n      \"example\": \"Zip\",\n      \"enum\": [\n        \"Zip\",\n        \"Image\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lambda/refs/heads/main/json-schema/amazon-lambda-function-schema.json
tags:
- Compute
- Event-Driven
- FaaS
- Functions
- Serverless
title: Function
---
