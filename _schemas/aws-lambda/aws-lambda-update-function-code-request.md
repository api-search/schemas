---
description: Request body for updating a function's code
layout: schema
name: UpdateFunctionCodeRequest
properties_list:
- description: Base64-encoded contents of the deployment package. AWS SDK and CLI clients handle encoding automatically.
  name: ZipFile
  type: string
- description: An S3 bucket in the same AWS Region as the function
  name: S3Bucket
  type: string
- description: The S3 key of the deployment package
  name: S3Key
  type: string
- description: For versioned S3 objects, the version of the deployment package
  name: S3ObjectVersion
  type: string
- description: URI of a container image in Amazon ECR
  name: ImageUri
  type: string
- description: Set to true to publish a new version of the function after updating the code
  name: Publish
  type: boolean
- description: Set to true to validate the request without updating the code
  name: DryRun
  type: boolean
- description: Update only if the revision ID matches
  name: RevisionId
  type: string
- description: ''
  name: Architectures
  type: array
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-update-function-code-request-schema.json
slug: aws-lambda-update-function-code-request
source_filename: aws-lambda-update-function-code-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateFunctionCodeRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a function's code\",\n  \"properties\": {\n    \"ZipFile\": {\n      \"type\": \"string\",\n      \"description\": \"Base64-encoded contents of the deployment package. AWS SDK and CLI clients handle encoding automatically.\"\n    },\n    \"S3Bucket\": {\n      \"type\": \"string\",\n      \"description\": \"An S3 bucket in the same AWS Region as the function\"\n    },\n    \"S3Key\": {\n      \"type\": \"string\",\n      \"description\": \"The S3 key of the deployment package\"\n    },\n    \"S3ObjectVersion\": {\n      \"type\": \"string\",\n      \"description\": \"For versioned S3 objects, the version of the deployment package\"\n    },\n    \"ImageUri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of a container image in Amazon ECR\"\n    },\n    \"Publish\": {\n      \"\
  type\": \"boolean\",\n      \"description\": \"Set to true to publish a new version of the function after updating the code\"\n    },\n    \"DryRun\": {\n      \"type\": \"boolean\",\n      \"description\": \"Set to true to validate the request without updating the code\"\n    },\n    \"RevisionId\": {\n      \"type\": \"string\",\n      \"description\": \"Update only if the revision ID matches\"\n    },\n    \"Architectures\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-update-function-code-request-schema.json
tags: []
title: UpdateFunctionCodeRequest
---
