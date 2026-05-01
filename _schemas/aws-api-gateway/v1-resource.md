---
description: Resource schema from Amazon API Gateway v1 API
layout: schema
name: Resource
properties_list:
- description: Resource identifier.
  name: id
  type: string
- description: Parent resource identifier.
  name: parentId
  type: string
- description: Last path segment for this resource.
  name: pathPart
  type: string
- description: Full path of the resource.
  name: path
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-resource-schema.json
slug: v1-resource
source_filename: v1-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Resource identifier.\",\n      \"example\": \"abc123\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent resource identifier.\",\n      \"example\": \"abc123\"\n    },\n    \"pathPart\": {\n      \"type\": \"string\",\n      \"description\": \"Last path segment for this resource.\",\n      \"example\": \"example-value\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Full path of the resource.\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-resource-schema.json\",\n  \"title\": \"Resource\",\n  \"description\": \"Resource schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-resource-schema.json
tags:
- API Gateway
- Cloud
- REST
- WebSocket
- Serverless
title: Resource
---
