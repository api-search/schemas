---
description: Schema representing an API gateway managed by the Apinizer platform
layout: schema
name: Apinizer Gateway
properties_list:
- description: Unique identifier of the gateway
  name: id
  type: string
- description: Name of the gateway
  name: name
  type: string
- description: Description of the gateway
  name: description
  type: string
- description: Base URL of the backend service
  name: baseUrl
  type: string
- description: Gateway status
  name: status
  type: string
- description: Creation timestamp
  name: createdAt
  type: string
provider_name: Apinizer
provider_slug: apinizer
schema_file: json-schema/apinizer-gateway-schema.json
slug: apinizer-gateway
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apinizer/main/json-schema/apinizer-gateway-schema.json\",\n  \"title\": \"Apinizer Gateway\",\n  \"description\": \"Schema representing an API gateway managed by the Apinizer platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique identifier of the gateway\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Name of the gateway\" },\n    \"description\": { \"type\": \"string\", \"description\": \"Description of the gateway\" },\n    \"baseUrl\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"Base URL of the backend service\" },\n    \"status\": { \"type\": \"string\", \"enum\": [\"active\", \"inactive\", \"maintenance\"], \"description\": \"Gateway status\" },\n    \"createdAt\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Creation\
  \ timestamp\" }\n  },\n  \"required\": [\"id\", \"name\", \"baseUrl\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apinizer/refs/heads/main/json-schema/apinizer-gateway-schema.json
tags:
- API Gateway
- API Management
- API Monitoring
- API Security
- Policies
title: Apinizer Gateway
---
