---
description: Response containing port-in request details
layout: schema
name: PortInResponse
properties_list:
- description: The unique identifier for the port-in request
  name: portInId
  type: string
- description: The current status of the port-in request
  name: status
  type: string
- description: The requested FOC date
  name: requestedFocDate
  type: string
- description: The actual FOC date assigned by the carrier
  name: actualFocDate
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-port-in-response-schema.json
slug: phone-numbers-port-in-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-port-in-response-schema.json\",\n  \"title\": \"PortInResponse\",\n  \"description\": \"Response containing port-in request details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portInId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the port-in request\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the port-in request\"\n    },\n    \"requestedFocDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The requested FOC date\"\n    },\n    \"actualFocDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The actual FOC date assigned by the carrier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-port-in-response-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: PortInResponse
---
