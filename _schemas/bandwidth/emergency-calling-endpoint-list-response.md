---
description: Response containing a list of E911 endpoints
layout: schema
name: EndpointListResponse
properties_list:
- description: Total number of endpoints
  name: totalCount
  type: integer
- description: ''
  name: endpoints
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/emergency-calling-endpoint-list-response-schema.json
slug: emergency-calling-endpoint-list-response
source_filename: emergency-calling-endpoint-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/emergency-calling-endpoint-list-response-schema.json\",\n  \"title\": \"EndpointListResponse\",\n  \"description\": \"Response containing a list of E911 endpoints\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of endpoints\"\n    },\n    \"endpoints\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Endpoint\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/emergency-calling-endpoint-list-response-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: EndpointListResponse
---
