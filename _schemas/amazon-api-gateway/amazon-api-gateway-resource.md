---
description: ''
layout: schema
name: Resource
properties_list:
- description: The resource's identifier.
  name: id
  type: string
- description: The parent resource's identifier.
  name: parentId
  type: string
- description: The last path segment for this resource.
  name: pathPart
  type: string
- description: The full path for this resource.
  name: path
  type: string
- description: Map of methods for this resource keyed by HTTP method type.
  name: resourceMethods
  type: object
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-resource-schema.json
slug: amazon-api-gateway-resource
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Resource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The resource's identifier.\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"The parent resource's identifier.\"\n    },\n    \"pathPart\": {\n      \"type\": \"string\",\n      \"description\": \"The last path segment for this resource.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The full path for this resource.\"\n    },\n    \"resourceMethods\": {\n      \"type\": \"object\",\n      \"description\": \"Map of methods for this resource keyed by HTTP method type.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-resource-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: Resource
---
