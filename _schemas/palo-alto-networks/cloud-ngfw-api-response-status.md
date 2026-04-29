---
description: Standard API response status envelope included in all responses.
layout: schema
name: ResponseStatus
properties_list:
- description: Error code. 0 indicates success.
  name: ErrorCode
  type: integer
- description: Human-readable status message.
  name: Reason
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-ngfw-api-response-status-schema.json
slug: cloud-ngfw-api-response-status
source_filename: cloud-ngfw-api-response-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseStatus\",\n  \"description\": \"Standard API response status envelope included in all responses.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-response-status-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ErrorCode\": {\n      \"type\": \"integer\",\n      \"description\": \"Error code. 0 indicates success.\",\n      \"example\": 0\n    },\n    \"Reason\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable status message.\",\n      \"example\": \"\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-response-status-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ResponseStatus
---
