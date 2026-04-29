---
description: Standard error response.
layout: schema
name: Error Response
properties_list:
- description: Error code or type.
  name: error
  type: string
- description: Human-readable error message.
  name: message
  type: string
- description: HTTP status code.
  name: status
  type: integer
provider_name: agilent-technologies
provider_slug: agilent-technologies
schema_file: json-schema/ilab-operations-api-error-response-schema.json
slug: ilab-operations-api-error-response
source_filename: ilab-operations-api-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-error-response-schema.json\",\n  \"title\": \"Error Response\",\n  \"description\": \"Standard error response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error code or type.\",\n      \"example\": \"not_found\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message.\",\n      \"example\": \"The requested resource was not found.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code.\",\n      \"example\": 404\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-error-response-schema.json
tags:
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
title: Error Response
---
