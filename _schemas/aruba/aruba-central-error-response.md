---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: Human-readable error message.
  name: description
  type: string
- description: Machine-readable error code.
  name: error_code
  type: string
- description: The API service that generated the error.
  name: service_name
  type: string
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-error-response-schema.json
slug: aruba-central-error-response
source_filename: aruba-central-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message.\"\n    },\n    \"error_code\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable error code.\"\n    },\n    \"service_name\": {\n      \"type\": \"string\",\n      \"description\": \"The API service that generated the error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-error-response-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: ErrorResponse
---
