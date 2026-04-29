---
description: Schema for an AWS Lambda function configuration. Defines the structure of a Lambda function resource including its code, runtime, execution role, memory, timeout, environment variables, VPC configuration, layers, concurrency, and other settings used by the Lambda service API.
layout: schema
name: AWS Lambda Function
properties_list:
- description: The name of the Lambda function. Can include letters, numbers, hyphens, and underscores. Must be between 1 and 64 characters.
  name: FunctionName
  type: string
- description: 'The function''s Amazon Resource Name (ARN). Format: arn:aws:lambda:{region}:{account-id}:function:{function-name}'
  name: FunctionArn
  type: string
- description: The identifier of the function's runtime. Required for .zip deployment packages. Not required for container image deployment packages.
  name: Runtime
  type: string
- description: The ARN of the function's execution role. This IAM role grants the function permission to access AWS services and resources.
  name: Role
  type: string
- description: The name of the method within your code that Lambda calls to run your function. The format includes the file name without an extension and the handler function or method name, separated by a dot (e.g.
  name: Handler
  type: string
- description: The size of the function's deployment package in bytes.
  name: CodeSize
  type: integer
- description: A description of the function's purpose.
  name: Description
  type: string
- description: The amount of time in seconds that Lambda allows a function to run before stopping it. The default is 3 seconds. The maximum allowed value is 900 seconds (15 minutes).
  name: Timeout
  type: integer
- description: The amount of memory available to the function at runtime in megabytes. Lambda allocates CPU power in proportion to the amount of memory configured. The default is 128 MB. The value can be any multipl
  name: MemorySize
  type: integer
- description: The date and time that the function was last updated, in ISO 8601 format (YYYY-MM-DDThh:mm:ss.sTZD).
  name: LastModified
  type: string
- description: The SHA-256 hash of the function's deployment package.
  name: CodeSha256
  type: string
- description: The version of the Lambda function. $LATEST for the unpublished version, or a numeric string for a published version.
  name: Version
  type: string
- description: The function's networking configuration for connecting to resources in a VPC
  name: VpcConfig
  type: object
- description: A dead-letter queue configuration that specifies the queue or topic where Lambda sends asynchronous events when they fail processing
  name: DeadLetterConfig
  type: object
- description: Environment variables that are accessible from function code during execution
  name: Environment
  type: object
- description: The ARN of the AWS KMS key used to encrypt the function's environment variables. If not provided, Lambda uses a default service key.
  name: KMSKeyArn
  type: string
- description: The function's AWS X-Ray tracing configuration
  name: TracingConfig
  type: object
- description: For Lambda@Edge functions, the ARN of the main function.
  name: MasterArn
  type: string
- description: The latest updated revision of the function or alias. Changes each time the function configuration or code is updated.
  name: RevisionId
  type: string
- description: A list of function layer ARNs (including version) applied to the function. Lambda applies layers in the order specified. Maximum of 5 layers.
  name: Layers
  type: array
- description: The current state of the function. When the state is Inactive, you can reactivate the function by invoking it.
  name: State
  type: string
- description: The reason for the function's current state.
  name: StateReason
  type: string
- description: The reason code for the function's current state. When the code is Creating, you cannot invoke or modify the function.
  name: StateReasonCode
  type: string
- description: The status of the last update that was performed on the function. Set to Successful after a function update completes.
  name: LastUpdateStatus
  type: string
- description: The reason for the last update that was performed on the function.
  name: LastUpdateStatusReason
  type: string
- description: The reason code for the last update that was performed on the function.
  name: LastUpdateStatusReasonCode
  type: string
- description: The type of deployment package. Zip for .zip file archive or Image for container image.
  name: PackageType
  type: string
- description: The function's image configuration values for container image deployment
  name: ImageConfigResponse
  type: object
- description: The instruction set architecture that the function supports. Lambda provides x86_64 (default) and arm64 (AWS Graviton2).
  name: Architectures
  type: array
- description: The size of the function's /tmp directory
  name: EphemeralStorage
  type: object
- description: SnapStart configuration to reduce cold start latency. Currently supported for Java runtime functions.
  name: SnapStart
  type: object
- description: The function's Amazon CloudWatch Logs configuration settings
  name: LoggingConfig
  type: object
- description: Key-value pairs attached to the function for organization, cost allocation, and access control.
  name: Tags
  type: object
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-function-schema.json
slug: aws-lambda-function
source_filename: aws-lambda-function-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.aws.amazon.com/lambda/schemas/function.json\",\n  \"title\": \"AWS Lambda Function\",\n  \"description\": \"Schema for an AWS Lambda function configuration. Defines the structure of a Lambda function resource including its code, runtime, execution role, memory, timeout, environment variables, VPC configuration, layers, concurrency, and other settings used by the Lambda service API.\",\n  \"type\": \"object\",\n  \"required\": [\"FunctionName\", \"Role\"],\n  \"properties\": {\n    \"FunctionName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Lambda function. Can include letters, numbers, hyphens, and underscores. Must be between 1 and 64 characters.\",\n      \"minLength\": 1,\n      \"maxLength\": 64,\n      \"pattern\": \"^[a-zA-Z0-9-_]+$\"\n    },\n    \"FunctionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The function's Amazon Resource\
  \ Name (ARN). Format: arn:aws:lambda:{region}:{account-id}:function:{function-name}\",\n      \"pattern\": \"^arn:aws:lambda:[a-z0-9-]+:[0-9]{12}:function:[a-zA-Z0-9-_]+(:[a-zA-Z0-9-_]+)?$\"\n    },\n    \"Runtime\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the function's runtime. Required for .zip deployment packages. Not required for container image deployment packages.\",\n      \"enum\": [\n        \"nodejs18.x\",\n        \"nodejs20.x\",\n        \"nodejs22.x\",\n        \"python3.9\",\n        \"python3.10\",\n        \"python3.11\",\n        \"python3.12\",\n        \"python3.13\",\n        \"java11\",\n        \"java17\",\n        \"java21\",\n        \"dotnet6\",\n        \"dotnet8\",\n        \"ruby3.2\",\n        \"ruby3.3\",\n        \"provided\",\n        \"provided.al2\",\n        \"provided.al2023\"\n      ]\n    },\n    \"Role\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the function's execution role. This IAM\
  \ role grants the function permission to access AWS services and resources.\",\n      \"pattern\": \"^arn:aws:iam::[0-9]{12}:role/.+$\"\n    },\n    \"Handler\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the method within your code that Lambda calls to run your function. The format includes the file name without an extension and the handler function or method name, separated by a dot (e.g., index.handler).\",\n      \"maxLength\": 128,\n      \"pattern\": \"^[a-zA-Z0-9._-]+$\"\n    },\n    \"CodeSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the function's deployment package in bytes.\",\n      \"minimum\": 0,\n      \"readOnly\": true\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the function's purpose.\",\n      \"maxLength\": 256\n    },\n    \"Timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of time in seconds that Lambda allows a function\
  \ to run before stopping it. The default is 3 seconds. The maximum allowed value is 900 seconds (15 minutes).\",\n      \"default\": 3,\n      \"minimum\": 1,\n      \"maximum\": 900\n    },\n    \"MemorySize\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of memory available to the function at runtime in megabytes. Lambda allocates CPU power in proportion to the amount of memory configured. The default is 128 MB. The value can be any multiple of 1 MB.\",\n      \"default\": 128,\n      \"minimum\": 128,\n      \"maximum\": 10240\n    },\n    \"LastModified\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time that the function was last updated, in ISO 8601 format (YYYY-MM-DDThh:mm:ss.sTZD).\",\n      \"readOnly\": true\n    },\n    \"CodeSha256\": {\n      \"type\": \"string\",\n      \"description\": \"The SHA-256 hash of the function's deployment package.\",\n      \"readOnly\": true\n    },\n    \"Version\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The version of the Lambda function. $LATEST for the unpublished version, or a numeric string for a published version.\",\n      \"readOnly\": true\n    },\n    \"VpcConfig\": {\n      \"$ref\": \"#/$defs/VpcConfig\",\n      \"description\": \"The function's networking configuration for connecting to resources in a VPC\"\n    },\n    \"DeadLetterConfig\": {\n      \"$ref\": \"#/$defs/DeadLetterConfig\",\n      \"description\": \"A dead-letter queue configuration that specifies the queue or topic where Lambda sends asynchronous events when they fail processing\"\n    },\n    \"Environment\": {\n      \"$ref\": \"#/$defs/Environment\",\n      \"description\": \"Environment variables that are accessible from function code during execution\"\n    },\n    \"KMSKeyArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the AWS KMS key used to encrypt the function's environment variables. If not provided, Lambda uses a default service key.\",\n  \
  \    \"pattern\": \"^arn:aws:kms:[a-z0-9-]+:[0-9]{12}:key/.+$\"\n    },\n    \"TracingConfig\": {\n      \"$ref\": \"#/$defs/TracingConfig\",\n      \"description\": \"The function's AWS X-Ray tracing configuration\"\n    },\n    \"MasterArn\": {\n      \"type\": \"string\",\n      \"description\": \"For Lambda@Edge functions, the ARN of the main function.\",\n      \"readOnly\": true\n    },\n    \"RevisionId\": {\n      \"type\": \"string\",\n      \"description\": \"The latest updated revision of the function or alias. Changes each time the function configuration or code is updated.\",\n      \"readOnly\": true\n    },\n    \"Layers\": {\n      \"type\": \"array\",\n      \"description\": \"A list of function layer ARNs (including version) applied to the function. Lambda applies layers in the order specified. Maximum of 5 layers.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"The ARN of a Lambda layer version\"\n      },\n      \"maxItems\": 5\n  \
  \  },\n    \"State\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the function. When the state is Inactive, you can reactivate the function by invoking it.\",\n      \"enum\": [\"Pending\", \"Active\", \"Inactive\", \"Failed\"],\n      \"readOnly\": true\n    },\n    \"StateReason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason for the function's current state.\",\n      \"readOnly\": true\n    },\n    \"StateReasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"The reason code for the function's current state. When the code is Creating, you cannot invoke or modify the function.\",\n      \"enum\": [\n        \"Idle\",\n        \"Creating\",\n        \"Restoring\",\n        \"EniLimitExceeded\",\n        \"InsufficientRolePermissions\",\n        \"InvalidConfiguration\",\n        \"InternalError\",\n        \"SubnetOutOfIPAddresses\",\n        \"InvalidSubnet\",\n        \"InvalidSecurityGroup\",\n        \"ImageDeleted\"\
  ,\n        \"ImageAccessDenied\",\n        \"InvalidImage\",\n        \"KMSKeyAccessDenied\",\n        \"KMSKeyNotFound\",\n        \"InvalidStateKMSKey\",\n        \"DisabledKMSKey\",\n        \"EFSIOError\",\n        \"EFSMountConnectivityError\",\n        \"EFSMountFailure\",\n        \"EFSMountTimeout\",\n        \"InvalidRuntime\",\n        \"InvalidZipFileException\",\n        \"FunctionError\"\n      ],\n      \"readOnly\": true\n    },\n    \"LastUpdateStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the last update that was performed on the function. Set to Successful after a function update completes.\",\n      \"enum\": [\"Successful\", \"Failed\", \"InProgress\"],\n      \"readOnly\": true\n    },\n    \"LastUpdateStatusReason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason for the last update that was performed on the function.\",\n      \"readOnly\": true\n    },\n    \"LastUpdateStatusReasonCode\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The reason code for the last update that was performed on the function.\",\n      \"readOnly\": true\n    },\n    \"PackageType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of deployment package. Zip for .zip file archive or Image for container image.\",\n      \"enum\": [\"Zip\", \"Image\"],\n      \"default\": \"Zip\"\n    },\n    \"ImageConfigResponse\": {\n      \"$ref\": \"#/$defs/ImageConfigResponse\",\n      \"description\": \"The function's image configuration values for container image deployment\"\n    },\n    \"Architectures\": {\n      \"type\": \"array\",\n      \"description\": \"The instruction set architecture that the function supports. Lambda provides x86_64 (default) and arm64 (AWS Graviton2).\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"x86_64\", \"arm64\"]\n      },\n      \"maxItems\": 1,\n      \"default\": [\"x86_64\"]\n    },\n    \"EphemeralStorage\": {\n      \"$ref\"\
  : \"#/$defs/EphemeralStorage\",\n      \"description\": \"The size of the function's /tmp directory\"\n    },\n    \"SnapStart\": {\n      \"$ref\": \"#/$defs/SnapStart\",\n      \"description\": \"SnapStart configuration to reduce cold start latency. Currently supported for Java runtime functions.\"\n    },\n    \"LoggingConfig\": {\n      \"$ref\": \"#/$defs/LoggingConfig\",\n      \"description\": \"The function's Amazon CloudWatch Logs configuration settings\"\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs attached to the function for organization, cost allocation, and access control.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"VpcConfig\": {\n      \"type\": \"object\",\n      \"description\": \"The VPC security groups and subnets that are attached to a Lambda function. When you connect a function to a VPC, Lambda creates an elastic network interface for each combination\
  \ of security group and subnet.\",\n      \"properties\": {\n        \"SubnetIds\": {\n          \"type\": \"array\",\n          \"description\": \"A list of VPC subnet IDs.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"pattern\": \"^subnet-[a-z0-9]+$\"\n          },\n          \"maxItems\": 16\n        },\n        \"SecurityGroupIds\": {\n          \"type\": \"array\",\n          \"description\": \"A list of VPC security group IDs.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"pattern\": \"^sg-[a-z0-9]+$\"\n          },\n          \"maxItems\": 5\n        },\n        \"VpcId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the VPC.\",\n          \"readOnly\": true\n        },\n        \"Ipv6AllowedForDualStack\": {\n          \"type\": \"boolean\",\n          \"description\": \"Allows outbound IPv6 traffic on VPC functions connected to dual-stack subnets.\"\n        }\n      }\n    },\n    \"DeadLetterConfig\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"The dead-letter queue for failed asynchronous invocations. An SQS queue or SNS topic destination.\",\n      \"properties\": {\n        \"TargetArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of an SQS queue or SNS topic.\",\n          \"pattern\": \"^arn:aws:(sqs|sns):[a-z0-9-]+:[0-9]{12}:.+$\"\n        }\n      }\n    },\n    \"Environment\": {\n      \"type\": \"object\",\n      \"description\": \"A function's environment variable settings. You can use environment variables to adjust your function's behavior without updating code.\",\n      \"properties\": {\n        \"Variables\": {\n          \"type\": \"object\",\n          \"description\": \"Environment variable key-value pairs. Keys can contain letters, numbers, and underscores. Total size of all environment variables cannot exceed 4 KB.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n\
  \        \"Error\": {\n          \"type\": \"object\",\n          \"description\": \"Error messages for environment variables that could not be applied.\",\n          \"readOnly\": true,\n          \"properties\": {\n            \"ErrorCode\": {\n              \"type\": \"string\"\n            },\n            \"Message\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"TracingConfig\": {\n      \"type\": \"object\",\n      \"description\": \"The function's AWS X-Ray tracing configuration. Set Mode to Active to sample incoming requests with X-Ray.\",\n      \"properties\": {\n        \"Mode\": {\n          \"type\": \"string\",\n          \"description\": \"The tracing mode. Active means Lambda samples a subset of invocations. PassThrough means Lambda only traces a request if an upstream service sends a trace header.\",\n          \"enum\": [\"Active\", \"PassThrough\"],\n          \"default\": \"PassThrough\"\n        }\n      }\n  \
  \  },\n    \"ImageConfigResponse\": {\n      \"type\": \"object\",\n      \"description\": \"Response structure for image configuration settings.\",\n      \"readOnly\": true,\n      \"properties\": {\n        \"ImageConfig\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"EntryPoint\": {\n              \"type\": \"array\",\n              \"description\": \"Specifies the entry point to the application, which is typically the location of the runtime executable.\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"maxItems\": 1500\n            },\n            \"Command\": {\n              \"type\": \"array\",\n              \"description\": \"Specifies parameters that you want to pass in with the ENTRYPOINT.\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"maxItems\": 1500\n            },\n            \"WorkingDirectory\": {\n              \"type\": \"\
  string\",\n              \"description\": \"Specifies the working directory.\",\n              \"maxLength\": 1000\n            }\n          }\n        },\n        \"Error\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"ErrorCode\": {\n              \"type\": \"string\"\n            },\n            \"Message\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"EphemeralStorage\": {\n      \"type\": \"object\",\n      \"description\": \"The size of the function's /tmp directory in MB. The default value is 512, but it can be any whole number between 512 and 10240 MB.\",\n      \"properties\": {\n        \"Size\": {\n          \"type\": \"integer\",\n          \"description\": \"The size of the /tmp directory in MB.\",\n          \"minimum\": 512,\n          \"maximum\": 10240,\n          \"default\": 512\n        }\n      },\n      \"required\": [\"Size\"]\n    },\n    \"SnapStart\": {\n      \"type\": \"\
  object\",\n      \"description\": \"The function's SnapStart setting. Lambda SnapStart creates a cached snapshot of the initialized execution environment to improve startup performance.\",\n      \"properties\": {\n        \"ApplyOn\": {\n          \"type\": \"string\",\n          \"description\": \"When set to PublishedVersions, Lambda creates a snapshot of the execution environment when you publish a function version.\",\n          \"enum\": [\"PublishedVersions\", \"None\"],\n          \"default\": \"None\"\n        },\n        \"OptimizationStatus\": {\n          \"type\": \"string\",\n          \"description\": \"When you provide a qualified ARN, this response element indicates whether SnapStart is activated for the specified function version.\",\n          \"enum\": [\"On\", \"Off\"],\n          \"readOnly\": true\n        }\n      }\n    },\n    \"LoggingConfig\": {\n      \"type\": \"object\",\n      \"description\": \"The function's Amazon CloudWatch Logs configuration settings.\"\
  ,\n      \"properties\": {\n        \"LogFormat\": {\n          \"type\": \"string\",\n          \"description\": \"The format in which Lambda sends function logs to CloudWatch. JSON format provides structured log output. Text format provides unstructured plaintext output.\",\n          \"enum\": [\"JSON\", \"Text\"],\n          \"default\": \"Text\"\n        },\n        \"ApplicationLogLevel\": {\n          \"type\": \"string\",\n          \"description\": \"Set this property to filter the application logs for your function that Lambda sends to CloudWatch. Only logs with a level at or above the selected level are sent.\",\n          \"enum\": [\"TRACE\", \"DEBUG\", \"INFO\", \"WARN\", \"ERROR\", \"FATAL\"]\n        },\n        \"SystemLogLevel\": {\n          \"type\": \"string\",\n          \"description\": \"Set this property to filter the system logs for your function that Lambda sends to CloudWatch.\",\n          \"enum\": [\"DEBUG\", \"INFO\", \"WARN\"]\n        },\n        \"LogGroup\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The name of the Amazon CloudWatch log group the function sends logs to. By default, Lambda functions send logs to /aws/lambda/{function-name}.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-function-schema.json
tags: []
title: AWS Lambda Function
---
