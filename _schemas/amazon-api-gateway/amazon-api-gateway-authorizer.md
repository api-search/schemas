---
description: ''
layout: schema
name: Authorizer
properties_list:
- description: The identifier of the authorizer.
  name: id
  type: string
- description: The name of the authorizer.
  name: name
  type: string
- description: The authorizer type.
  name: type
  type: string
- description: A list of the Amazon Cognito user pool ARNs.
  name: providerARNs
  type: array
- description: An optional customer-defined field for authorization type.
  name: authType
  type: string
- description: The authorizer's URI. For TOKEN or REQUEST authorizers, this is the Lambda function URI.
  name: authorizerUri
  type: string
- description: The credentials required for the authorizer as an IAM role ARN.
  name: authorizerCredentials
  type: string
- description: The identity source for which authorization is requested.
  name: identitySource
  type: string
- description: A validation expression for the incoming identity token.
  name: identityValidationExpression
  type: string
- description: The TTL in seconds of cached authorizer results. Max 3600.
  name: authorizerResultTtlInSeconds
  type: integer
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-authorizer-schema.json
slug: amazon-api-gateway-authorizer
source_filename: amazon-api-gateway-authorizer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Authorizer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the authorizer.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the authorizer.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The authorizer type.\",\n      \"enum\": [\n        \"TOKEN\",\n        \"REQUEST\",\n        \"COGNITO_USER_POOLS\"\n      ]\n    },\n    \"providerARNs\": {\n      \"type\": \"array\",\n      \"description\": \"A list of the Amazon Cognito user pool ARNs.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"authType\": {\n      \"type\": \"string\",\n      \"description\": \"An optional customer-defined field for authorization type.\"\n    },\n    \"authorizerUri\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The authorizer's URI. For TOKEN or REQUEST authorizers, this is the Lambda function URI.\"\n    },\n    \"authorizerCredentials\": {\n      \"type\": \"string\",\n      \"description\": \"The credentials required for the authorizer as an IAM role ARN.\"\n    },\n    \"identitySource\": {\n      \"type\": \"string\",\n      \"description\": \"The identity source for which authorization is requested.\"\n    },\n    \"identityValidationExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A validation expression for the incoming identity token.\"\n    },\n    \"authorizerResultTtlInSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"The TTL in seconds of cached authorizer results. Max 3600.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-authorizer-schema.json
tags:
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: Authorizer
---
