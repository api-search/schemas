---
description: An E911 endpoint representing an end user
layout: schema
name: Endpoint
properties_list:
- description: The unique identifier for the endpoint
  name: endpointId
  type: string
- description: The Alternate End User ID (AEUI) that identifies the end user
  name: alternateEndUserId
  type: string
- description: The name of the end user for PSAP display
  name: callerName
  type: string
- description: The ID of the validated location associated with this endpoint
  name: locationId
  type: string
- description: The phone number associated with this endpoint
  name: telephoneNumber
  type: string
- description: Whether the endpoint is currently active
  name: activated
  type: boolean
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/emergency-calling-endpoint-schema.json
slug: emergency-calling-endpoint
source_filename: emergency-calling-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/emergency-calling-endpoint-schema.json\",\n  \"title\": \"Endpoint\",\n  \"description\": \"An E911 endpoint representing an end user\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endpointId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the endpoint\"\n    },\n    \"alternateEndUserId\": {\n      \"type\": \"string\",\n      \"description\": \"The Alternate End User ID (AEUI) that identifies the end user\"\n    },\n    \"callerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the end user for PSAP display\"\n    },\n    \"locationId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the validated location associated with this endpoint\"\n    },\n    \"telephoneNumber\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The phone number associated with this endpoint\"\n    },\n    \"activated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the endpoint is currently active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/emergency-calling-endpoint-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Endpoint
---
