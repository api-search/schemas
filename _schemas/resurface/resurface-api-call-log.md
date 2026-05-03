---
description: A complete API call log record captured by the Resurface runtime security platform, including full request and response payload data.
layout: schema
name: Resurface API Call Log
properties_list:
- description: Unique identifier for this API call log record.
  name: id
  type: string
- description: The HTTP method of the request.
  name: request_method
  type: string
- description: The full URL of the API request.
  name: request_url
  type: string
- description: Request headers as key-value pairs.
  name: request_header
  type: array
- description: The full request body payload.
  name: request_body
  type: string
- description: The HTTP status code of the response.
  name: response_code
  type: integer
- description: Response headers as key-value pairs.
  name: response_header
  type: array
- description: The full response body payload.
  name: response_body
  type: string
- description: Time taken to process the request in milliseconds.
  name: interval_millis
  type: integer
- description: The hostname that received and processed the API call.
  name: host
  type: string
- description: Timestamp when the API call was captured, in milliseconds since epoch.
  name: now
  type: string
- description: Custom session fields attached to this log record.
  name: session_field
  type: array
provider_name: Resurface
provider_slug: resurface
schema_file: json-schema/resurface-api-call-log-schema.json
slug: resurface-api-call-log
source_filename: resurface-api-call-log-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/resurface/json-schema/resurface-api-call-log-schema.json\",\n  \"title\": \"Resurface API Call Log\",\n  \"description\": \"A complete API call log record captured by the Resurface runtime security platform, including full request and response payload data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this API call log record.\"\n    },\n    \"request_method\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP method of the request.\",\n      \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\", \"HEAD\", \"OPTIONS\", \"TRACE\"]\n    },\n    \"request_url\": {\n      \"type\": \"string\",\n      \"description\": \"The full URL of the API request.\"\n    },\n    \"request_header\": {\n      \"type\": \"array\",\n      \"description\": \"Request\
  \ headers as key-value pairs.\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": { \"type\": \"string\" },\n        \"minItems\": 2,\n        \"maxItems\": 2\n      }\n    },\n    \"request_body\": {\n      \"type\": \"string\",\n      \"description\": \"The full request body payload.\"\n    },\n    \"response_code\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP status code of the response.\"\n    },\n    \"response_header\": {\n      \"type\": \"array\",\n      \"description\": \"Response headers as key-value pairs.\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": { \"type\": \"string\" },\n        \"minItems\": 2,\n        \"maxItems\": 2\n      }\n    },\n    \"response_body\": {\n      \"type\": \"string\",\n      \"description\": \"The full response body payload.\"\n    },\n    \"interval_millis\": {\n      \"type\": \"integer\",\n      \"description\": \"Time taken to process the request in milliseconds.\"\n    },\n\
  \    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname that received and processed the API call.\"\n    },\n    \"now\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the API call was captured, in milliseconds since epoch.\"\n    },\n    \"session_field\": {\n      \"type\": \"array\",\n      \"description\": \"Custom session fields attached to this log record.\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": { \"type\": \"string\" },\n        \"minItems\": 2,\n        \"maxItems\": 2\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/resurface/refs/heads/main/json-schema/resurface-api-call-log-schema.json
tags:
- API Analytics
- API Compliance
- API Logging
- API Observability
- API Security
- Data Leak Prevention
- Runtime Security
- SIEM
- Threat Detection
title: Resurface API Call Log
---
