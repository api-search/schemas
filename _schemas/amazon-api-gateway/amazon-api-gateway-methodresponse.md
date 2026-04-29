---
description: ''
layout: schema
name: MethodResponse
properties_list:
- description: The method response's status code.
  name: statusCode
  type: string
- description: ''
  name: responseParameters
  type: object
- description: ''
  name: responseModels
  type: object
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-methodresponse-schema.json
slug: amazon-api-gateway-methodresponse
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"MethodResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statusCode\": {\n      \"type\": \"string\",\n      \"description\": \"The method response's status code.\"\n    },\n    \"responseParameters\": {\n      \"type\": \"object\"\n    },\n    \"responseModels\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-methodresponse-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: MethodResponse
---
