---
description: ''
layout: schema
name: IntegrationResponse
properties_list:
- description: ''
  name: statusCode
  type: string
- description: ''
  name: selectionPattern
  type: string
- description: ''
  name: responseParameters
  type: object
- description: ''
  name: responseTemplates
  type: object
- description: ''
  name: contentHandling
  type: string
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-integrationresponse-schema.json
slug: amazon-api-gateway-integrationresponse
source_filename: amazon-api-gateway-integrationresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"IntegrationResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statusCode\": {\n      \"type\": \"string\"\n    },\n    \"selectionPattern\": {\n      \"type\": \"string\"\n    },\n    \"responseParameters\": {\n      \"type\": \"object\"\n    },\n    \"responseTemplates\": {\n      \"type\": \"object\"\n    },\n    \"contentHandling\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CONVERT_TO_BINARY\",\n        \"CONVERT_TO_TEXT\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-integrationresponse-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: IntegrationResponse
---
