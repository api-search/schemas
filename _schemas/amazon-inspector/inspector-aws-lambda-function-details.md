---
description: A summary of information about the AWS Lambda function.
layout: schema
name: AwsLambdaFunctionDetails
properties_list:
- description: ''
  name: architectures
  type: object
- description: ''
  name: codeSha256
  type: object
- description: ''
  name: executionRoleArn
  type: object
- description: ''
  name: functionName
  type: object
- description: ''
  name: lastModifiedAt
  type: object
- description: ''
  name: layers
  type: object
- description: ''
  name: packageType
  type: object
- description: ''
  name: runtime
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: vpcConfig
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-aws-lambda-function-details-schema.json
slug: inspector-aws-lambda-function-details
source_filename: inspector-aws-lambda-function-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-aws-lambda-function-details-schema.json\",\n  \"title\": \"AwsLambdaFunctionDetails\",\n  \"description\": \" A summary of information about the AWS Lambda function.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"architectures\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArchitectureList\"\n        },\n        {\n          \"description\": \"The instruction set architecture that the AWS Lambda function supports. Architecture is a string array with one of the valid values. The default architecture value is <code>x86_64</code>.\"\n        }\n      ]\n    },\n    \"codeSha256\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The SHA256 hash of the AWS Lambda\
  \ function's deployment package.\"\n        }\n      ]\n    },\n    \"executionRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionRoleArn\"\n        },\n        {\n          \"description\": \"The AWS Lambda function's execution role.\"\n        }\n      ]\n    },\n    \"functionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FunctionName\"\n        },\n        {\n          \"description\": \"The name of the AWS Lambda function.\"\n        }\n      ]\n    },\n    \"lastModifiedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time that a user last updated the configuration, in <a href=\\\"https://www.iso.org/iso-8601-date-and-time-format.html\\\">ISO 8601 format</a> \"\n        }\n      ]\n    },\n    \"layers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LayerList\"\
  \n        },\n        {\n          \"description\": \"The AWS Lambda function's <a href=\\\"https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html\\\"> layers</a>. A Lambda function can have up to five layers.\"\n        }\n      ]\n    },\n    \"packageType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageType\"\n        },\n        {\n          \"description\": \"The type of deployment package. Set to <code>Image</code> for container image and set <code>Zip</code> for .zip file archive.\"\n        }\n      ]\n    },\n    \"runtime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Runtime\"\n        },\n        {\n          \"description\": \"The runtime environment for the AWS Lambda function.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version of the AWS\
  \ Lambda function.\"\n        }\n      ]\n    },\n    \"vpcConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaVpcConfig\"\n        },\n        {\n          \"description\": \"The AWS Lambda function's networking configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"codeSha256\",\n    \"executionRoleArn\",\n    \"functionName\",\n    \"runtime\",\n    \"version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-aws-lambda-function-details-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AwsLambdaFunctionDetails
---
