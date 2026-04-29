---
description: ''
layout: schema
name: Integration
properties_list:
- description: The integration input's type.
  name: type
  type: string
- description: The integration's HTTP method type.
  name: httpMethod
  type: string
- description: The Uniform Resource Identifier (URI) for the integration.
  name: uri
  type: string
- description: The type of the network connection to the integration endpoint.
  name: connectionType
  type: string
- description: The ID of the VPC link used for the integration when connectionType is VPC_LINK.
  name: connectionId
  type: string
- description: The credentials required for the integration, if any. For AWS integrations, three options are available.
  name: credentials
  type: string
- description: ''
  name: requestParameters
  type: object
- description: ''
  name: requestTemplates
  type: object
- description: ''
  name: passthroughBehavior
  type: string
- description: ''
  name: contentHandling
  type: string
- description: Custom timeout between 50 and 29000 milliseconds.
  name: timeoutInMillis
  type: integer
- description: ''
  name: cacheNamespace
  type: string
- description: ''
  name: cacheKeyParameters
  type: array
- description: ''
  name: integrationResponses
  type: object
- description: ''
  name: tlsConfig
  type: object
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-integration-schema.json
slug: amazon-api-gateway-integration
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Integration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The integration input's type.\",\n      \"enum\": [\n        \"HTTP\",\n        \"HTTP_PROXY\",\n        \"AWS\",\n        \"AWS_PROXY\",\n        \"MOCK\"\n      ]\n    },\n    \"httpMethod\": {\n      \"type\": \"string\",\n      \"description\": \"The integration's HTTP method type.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"The Uniform Resource Identifier (URI) for the integration.\"\n    },\n    \"connectionType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the network connection to the integration endpoint.\",\n      \"enum\": [\n        \"INTERNET\",\n        \"VPC_LINK\"\n      ]\n    },\n    \"connectionId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the VPC link used for\
  \ the integration when connectionType is VPC_LINK.\"\n    },\n    \"credentials\": {\n      \"type\": \"string\",\n      \"description\": \"The credentials required for the integration, if any. For AWS integrations, three options are available.\"\n    },\n    \"requestParameters\": {\n      \"type\": \"object\"\n    },\n    \"requestTemplates\": {\n      \"type\": \"object\"\n    },\n    \"passthroughBehavior\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"WHEN_NO_MATCH\",\n        \"WHEN_NO_TEMPLATES\",\n        \"NEVER\"\n      ]\n    },\n    \"contentHandling\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CONVERT_TO_BINARY\",\n        \"CONVERT_TO_TEXT\"\n      ]\n    },\n    \"timeoutInMillis\": {\n      \"type\": \"integer\",\n      \"description\": \"Custom timeout between 50 and 29000 milliseconds.\"\n    },\n    \"cacheNamespace\": {\n      \"type\": \"string\"\n    },\n    \"cacheKeyParameters\": {\n      \"type\": \"array\",\n      \"items\":\
  \ {\n        \"type\": \"string\"\n      }\n    },\n    \"integrationResponses\": {\n      \"type\": \"object\"\n    },\n    \"tlsConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"insecureSkipVerification\": {\n          \"type\": \"boolean\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-integration-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: Integration
---
