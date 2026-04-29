---
description: Response containing a list of port-in requests
layout: schema
name: PortInListResponse
properties_list:
- description: Total number of port-in requests
  name: totalCount
  type: integer
- description: ''
  name: portIns
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-port-in-list-response-schema.json
slug: phone-numbers-port-in-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-port-in-list-response-schema.json\",\n  \"title\": \"PortInListResponse\",\n  \"description\": \"Response containing a list of port-in requests\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of port-in requests\"\n    },\n    \"portIns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PortInResponse\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-port-in-list-response-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: PortInListResponse
---
