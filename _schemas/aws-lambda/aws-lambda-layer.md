---
description: An Lambda layer attached to a function
layout: schema
name: Layer
properties_list:
- description: The ARN of the function layer
  name: Arn
  type: string
- description: The size of the layer archive in bytes
  name: CodeSize
  type: integer
- description: The ARN of a signing profile version
  name: SigningProfileVersionArn
  type: string
- description: The ARN of a signing job
  name: SigningJobArn
  type: string
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-layer-schema.json
slug: aws-lambda-layer
source_filename: aws-lambda-layer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Layer\",\n  \"type\": \"object\",\n  \"description\": \"An Lambda layer attached to a function\",\n  \"properties\": {\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the function layer\"\n    },\n    \"CodeSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the layer archive in bytes\"\n    },\n    \"SigningProfileVersionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of a signing profile version\"\n    },\n    \"SigningJobArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of a signing job\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-layer-schema.json
tags: []
title: Layer
---
