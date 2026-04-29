---
description: Standard PAN-OS API response envelope.
layout: schema
name: PanOsResponse
properties_list:
- description: ''
  name: '@status'
  type: string
- description: ''
  name: '@code'
  type: string
- description: ''
  name: msg
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/pan-os-rest-api-pan-os-response-schema.json
slug: pan-os-rest-api-pan-os-response
source_filename: pan-os-rest-api-pan-os-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PanOsResponse\",\n  \"description\": \"Standard PAN-OS API response envelope.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-pan-os-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"success\",\n        \"error\"\n      ]\n    },\n    \"@code\": {\n      \"type\": \"string\"\n    },\n    \"msg\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-pan-os-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: PanOsResponse
---
