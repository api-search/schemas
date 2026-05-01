---
description: ''
layout: schema
name: CreateDocumentationPartRequest
properties_list:
- description: ''
  name: location
  type: object
- description: ''
  name: properties
  type: string
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-createdocumentationpartrequest-schema.json
slug: amazon-api-gateway-createdocumentationpartrequest
source_filename: amazon-api-gateway-createdocumentationpartrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateDocumentationPartRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"location\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"API\",\n            \"AUTHORIZER\",\n            \"MODEL\",\n            \"RESOURCE\",\n            \"METHOD\",\n            \"PATH_PARAMETER\",\n            \"QUERY_PARAMETER\",\n            \"REQUEST_HEADER\",\n            \"REQUEST_BODY\",\n            \"RESPONSE\",\n            \"RESPONSE_HEADER\",\n            \"RESPONSE_BODY\"\n          ]\n        },\n        \"path\": {\n          \"type\": \"string\"\n        },\n        \"method\": {\n          \"type\": \"string\"\n        },\n        \"statusCode\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"properties\"\
  : {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"location\",\n    \"properties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-createdocumentationpartrequest-schema.json
tags:
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: CreateDocumentationPartRequest
---
