---
description: EndpointConfiguration schema from Amazon API Gateway v1 API
layout: schema
name: EndpointConfiguration
properties_list:
- description: List of endpoint types (EDGE, REGIONAL, PRIVATE).
  name: types
  type: array
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-endpoint-configuration-schema.json
slug: v1-endpoint-configuration
source_filename: v1-endpoint-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"types\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"EDGE\",\n          \"REGIONAL\",\n          \"PRIVATE\"\n        ]\n      },\n      \"description\": \"List of endpoint types (EDGE, REGIONAL, PRIVATE).\",\n      \"example\": [\n        \"EDGE\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-endpoint-configuration-schema.json\",\n  \"title\": \"EndpointConfiguration\",\n  \"description\": \"EndpointConfiguration schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-endpoint-configuration-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: EndpointConfiguration
---
