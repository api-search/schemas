---
description: Response containing a list of E911 locations
layout: schema
name: LocationListResponse
properties_list:
- description: Total number of locations
  name: totalCount
  type: integer
- description: ''
  name: locations
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/emergency-calling-location-list-response-schema.json
slug: emergency-calling-location-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/emergency-calling-location-list-response-schema.json\",\n  \"title\": \"LocationListResponse\",\n  \"description\": \"Response containing a list of E911 locations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of locations\"\n    },\n    \"locations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Location\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/emergency-calling-location-list-response-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: LocationListResponse
---
