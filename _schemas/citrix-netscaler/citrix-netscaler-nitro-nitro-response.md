---
description: Standard NITRO API success response.
layout: schema
name: NitroResponse
properties_list:
- description: Error code. 0 indicates success.
  name: errorcode
  type: integer
- description: Human-readable message describing the result.
  name: message
  type: string
- description: Severity level of the response.
  name: severity
  type: string
provider_name: Citrix NetScaler
provider_slug: citrix-netscaler
schema_file: json-schema/citrix-netscaler-nitro-nitro-response-schema.json
slug: citrix-netscaler-nitro-nitro-response
source_filename: citrix-netscaler-nitro-nitro-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NitroResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard NITRO API success response.\",\n  \"properties\": {\n    \"errorcode\": {\n      \"type\": \"integer\",\n      \"description\": \"Error code. 0 indicates success.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable message describing the result.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Severity level of the response.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/json-schema/citrix-netscaler-nitro-nitro-response-schema.json
tags:
- API Gateway
- Application Delivery Controller
- Application Security
- Load Balancing
- SSL Offloading
- Traffic Management
- Web Application Firewall
title: NitroResponse
---
