---
description: Quality on Demand session details and status
layout: schema
name: QoD Session Info
properties_list:
- description: ''
  name: sessionId
  type: string
- description: ''
  name: qosProfile
  type: string
- description: ''
  name: qosStatus
  type: string
- description: ''
  name: expiresAt
  type: string
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/network-apis-session-info-schema.json
slug: network-apis-session-info
source_filename: network-apis-session-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.att.com/schemas/network/session-info\",\n  \"title\": \"QoD Session Info\",\n  \"description\": \"Quality on Demand session details and status\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessionId\": {\n      \"type\": \"string\"\n    },\n    \"qosProfile\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"LOW_LATENCY\",\n        \"THROUGHPUT_S\",\n        \"THROUGHPUT_M\",\n        \"THROUGHPUT_L\",\n        \"VOICE\"\n      ]\n    },\n    \"qosStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"REQUESTED\",\n        \"AVAILABLE\",\n        \"UNAVAILABLE\"\n      ]\n    },\n    \"expiresAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/network-apis-session-info-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: QoD Session Info
---
