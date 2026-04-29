---
description: NITRO API error response with details about the failure.
layout: schema
name: NitroErrorResponse
properties_list:
- description: Numeric error code identifying the specific error.
  name: errorcode
  type: integer
- description: Human-readable error message.
  name: message
  type: string
- description: Severity level of the error.
  name: severity
  type: string
provider_name: Citrix NetScaler
provider_slug: citrix-netscaler
schema_file: json-schema/citrix-netscaler-nitro-nitro-error-response-schema.json
slug: citrix-netscaler-nitro-nitro-error-response
source_filename: citrix-netscaler-nitro-nitro-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NitroErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"NITRO API error response with details about the failure.\",\n  \"properties\": {\n    \"errorcode\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric error code identifying the specific error.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Severity level of the error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/json-schema/citrix-netscaler-nitro-nitro-error-response-schema.json
tags:
- API Gateway
- Application Delivery Controller
- Application Security
- Load Balancing
- SSL Offloading
- Traffic Management
- Web Application Firewall
title: NitroErrorResponse
---
