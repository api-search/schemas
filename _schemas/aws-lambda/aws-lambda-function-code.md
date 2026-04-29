---
description: The code for the Lambda function. You can provide your deployment package as a .zip file archive uploaded directly, from S3, or as a container image from Amazon ECR.
layout: schema
name: FunctionCode
properties_list:
- description: Base64-encoded contents of the deployment package .zip file
  name: ZipFile
  type: string
- description: An S3 bucket in the same AWS Region as your function
  name: S3Bucket
  type: string
- description: The S3 key of the deployment package
  name: S3Key
  type: string
- description: The version of the S3 object for versioned buckets
  name: S3ObjectVersion
  type: string
- description: URI of a container image in the Amazon ECR registry
  name: ImageUri
  type: string
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-function-code-schema.json
slug: aws-lambda-function-code
source_filename: aws-lambda-function-code-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FunctionCode\",\n  \"type\": \"object\",\n  \"description\": \"The code for the Lambda function. You can provide your deployment package as a .zip file archive uploaded directly, from S3, or as a container image from Amazon ECR.\",\n  \"properties\": {\n    \"ZipFile\": {\n      \"type\": \"string\",\n      \"description\": \"Base64-encoded contents of the deployment package .zip file\"\n    },\n    \"S3Bucket\": {\n      \"type\": \"string\",\n      \"description\": \"An S3 bucket in the same AWS Region as your function\"\n    },\n    \"S3Key\": {\n      \"type\": \"string\",\n      \"description\": \"The S3 key of the deployment package\"\n    },\n    \"S3ObjectVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the S3 object for versioned buckets\"\n    },\n    \"ImageUri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of a container image in\
  \ the Amazon ECR registry\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-function-code-schema.json
tags: []
title: FunctionCode
---
