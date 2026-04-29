---
description: A Lambda function's configuration and metadata
layout: schema
name: FunctionConfiguration
properties_list:
- description: The name of the function
  name: FunctionName
  type: string
- description: The function's Amazon Resource Name (ARN)
  name: FunctionArn
  type: string
- description: The identifier of the function's runtime. Runtime is required if the deployment package is a .zip file archive.
  name: Runtime
  type: string
- description: The function's execution role ARN
  name: Role
  type: string
- description: The function entrypoint in your code. The format includes the file name without extension and the handler function name (e.g. index.handler)
  name: Handler
  type: string
- description: The size of the function's deployment package in bytes
  name: CodeSize
  type: integer
- description: The function's description
  name: Description
  type: string
- description: The amount of time in seconds that Lambda allows a function to run before stopping it. Maximum is 900 seconds (15 minutes).
  name: Timeout
  type: integer
- description: The amount of memory available to the function at runtime in MB. Lambda allocates CPU power in proportion to the amount of memory configured.
  name: MemorySize
  type: integer
- description: The date and time the function was last updated in ISO 8601 format
  name: LastModified
  type: string
- description: The SHA-256 hash of the function's deployment package
  name: CodeSha256
  type: string
- description: The version of the Lambda function
  name: Version
  type: string
- description: The function's dead-letter queue configuration
  name: DeadLetterConfig
  type: object
- description: The function's environment variables
  name: Environment
  type: object
- description: The ARN of the KMS key used to encrypt the function's environment variables at rest
  name: KMSKeyArn
  type: string
- description: The function's X-Ray tracing configuration
  name: TracingConfig
  type: object
- description: For Lambda@Edge functions, the ARN of the main function
  name: MasterArn
  type: string
- description: The latest updated revision of the function
  name: RevisionId
  type: string
- description: The function's layers
  name: Layers
  type: array
- description: The current state of the function
  name: State
  type: string
- description: The reason for the function's current state
  name: StateReason
  type: string
- description: The reason code for the function's current state
  name: StateReasonCode
  type: string
- description: The status of the last update that was performed on the function
  name: LastUpdateStatus
  type: string
- description: The reason for the last update that was performed on the function
  name: LastUpdateStatusReason
  type: string
- description: The reason code for the last update
  name: LastUpdateStatusReasonCode
  type: string
- description: The type of deployment package
  name: PackageType
  type: string
- description: The function's image configuration values for container images
  name: ImageConfigResponse
  type: object
- description: The instruction set architecture that the function supports
  name: Architectures
  type: array
- description: The size of the function's /tmp directory in MB
  name: EphemeralStorage
  type: object
- description: The function's SnapStart setting for reducing cold start latency
  name: SnapStart
  type: object
- description: The ARN of the runtime and any errors that occurred
  name: RuntimeVersionConfig
  type: object
- description: The function's Amazon CloudWatch Logs configuration
  name: LoggingConfig
  type: object
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-function-configuration-schema.json
slug: aws-lambda-function-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FunctionConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"A Lambda function's configuration and metadata\",\n  \"properties\": {\n    \"FunctionName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the function\"\n    },\n    \"FunctionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The function's Amazon Resource Name (ARN)\"\n    },\n    \"Runtime\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the function's runtime. Runtime is required if the deployment package is a .zip file archive.\"\n    },\n    \"Role\": {\n      \"type\": \"string\",\n      \"description\": \"The function's execution role ARN\"\n    },\n    \"Handler\": {\n      \"type\": \"string\",\n      \"description\": \"The function entrypoint in your code. The format includes the file name without extension and the handler function name (e.g. index.handler)\"\
  \n    },\n    \"CodeSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the function's deployment package in bytes\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The function's description\"\n    },\n    \"Timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of time in seconds that Lambda allows a function to run before stopping it. Maximum is 900 seconds (15 minutes).\"\n    },\n    \"MemorySize\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of memory available to the function at runtime in MB. Lambda allocates CPU power in proportion to the amount of memory configured.\"\n    },\n    \"LastModified\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the function was last updated in ISO 8601 format\"\n    },\n    \"CodeSha256\": {\n      \"type\": \"string\",\n      \"description\": \"The SHA-256 hash of the function's deployment package\"\n\
  \    },\n    \"Version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the Lambda function\"\n    },\n    \"DeadLetterConfig\": {\n      \"type\": \"object\",\n      \"description\": \"The function's dead-letter queue configuration\"\n    },\n    \"Environment\": {\n      \"type\": \"object\",\n      \"description\": \"The function's environment variables\"\n    },\n    \"KMSKeyArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the KMS key used to encrypt the function's environment variables at rest\"\n    },\n    \"TracingConfig\": {\n      \"type\": \"object\",\n      \"description\": \"The function's X-Ray tracing configuration\"\n    },\n    \"MasterArn\": {\n      \"type\": \"string\",\n      \"description\": \"For Lambda@Edge functions, the ARN of the main function\"\n    },\n    \"RevisionId\": {\n      \"type\": \"string\",\n      \"description\": \"The latest updated revision of the function\"\n    },\n    \"Layers\": {\n    \
  \  \"type\": \"array\",\n      \"description\": \"The function's layers\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the function\"\n    },\n    \"StateReason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason for the function's current state\"\n    },\n    \"StateReasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"The reason code for the function's current state\"\n    },\n    \"LastUpdateStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the last update that was performed on the function\"\n    },\n    \"LastUpdateStatusReason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason for the last update that was performed on the function\"\n    },\n    \"LastUpdateStatusReasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"The reason code for the last update\"\n    },\n    \"PackageType\": {\n      \"type\": \"string\",\n      \"\
  description\": \"The type of deployment package\"\n    },\n    \"ImageConfigResponse\": {\n      \"type\": \"object\",\n      \"description\": \"The function's image configuration values for container images\"\n    },\n    \"Architectures\": {\n      \"type\": \"array\",\n      \"description\": \"The instruction set architecture that the function supports\"\n    },\n    \"EphemeralStorage\": {\n      \"type\": \"object\",\n      \"description\": \"The size of the function's /tmp directory in MB\"\n    },\n    \"SnapStart\": {\n      \"type\": \"object\",\n      \"description\": \"The function's SnapStart setting for reducing cold start latency\"\n    },\n    \"RuntimeVersionConfig\": {\n      \"type\": \"object\",\n      \"description\": \"The ARN of the runtime and any errors that occurred\"\n    },\n    \"LoggingConfig\": {\n      \"type\": \"object\",\n      \"description\": \"The function's Amazon CloudWatch Logs configuration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-function-configuration-schema.json
tags: []
title: FunctionConfiguration
---
