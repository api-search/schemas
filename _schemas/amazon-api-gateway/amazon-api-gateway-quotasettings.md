---
description: ''
layout: schema
name: QuotaSettings
properties_list:
- description: The maximum number of requests per time period.
  name: limit
  type: integer
- description: The day that a time period starts.
  name: offset
  type: integer
- description: The time period for which the maximum limit applies.
  name: period
  type: string
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-quotasettings-schema.json
slug: amazon-api-gateway-quotasettings
source_filename: amazon-api-gateway-quotasettings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"QuotaSettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of requests per time period.\"\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"The day that a time period starts.\"\n    },\n    \"period\": {\n      \"type\": \"string\",\n      \"description\": \"The time period for which the maximum limit applies.\",\n      \"enum\": [\n        \"DAY\",\n        \"WEEK\",\n        \"MONTH\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-quotasettings-schema.json
tags:
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: QuotaSettings
---
