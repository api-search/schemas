---
description: Configuration for Lambda-based authorization
layout: schema
name: LambdaAuthorizerConfig
properties_list:
- description: Lambda function ARN
  name: authorizerUri
  type: string
- description: TTL for authorizer results in seconds
  name: authorizerResultTtlInSeconds
  type: integer
- description: Regular expression for validating tokens
  name: identityValidationExpression
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-lambda-authorizer-config-schema.json
slug: appsync-lambda-authorizer-config
source_filename: appsync-lambda-authorizer-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-lambda-authorizer-config-schema.json\",\n  \"title\": \"LambdaAuthorizerConfig\",\n  \"description\": \"Configuration for Lambda-based authorization\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorizerUri\": {\n      \"type\": \"string\",\n      \"description\": \"Lambda function ARN\"\n    },\n    \"authorizerResultTtlInSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"TTL for authorizer results in seconds\"\n    },\n    \"identityValidationExpression\": {\n      \"type\": \"string\",\n      \"description\": \"Regular expression for validating tokens\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-lambda-authorizer-config-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: LambdaAuthorizerConfig
---
