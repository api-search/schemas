---
description: Request to create a Quality on Demand session
layout: schema
name: Create QoD Session Request
properties_list:
- description: ''
  name: phoneNumber
  type: string
- description: ''
  name: qosProfile
  type: string
- description: ''
  name: duration
  type: integer
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/network-apis-create-session-request-schema.json
slug: network-apis-create-session-request
source_filename: network-apis-create-session-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.att.com/schemas/network/create-session-request\",\n  \"title\": \"Create QoD Session Request\",\n  \"description\": \"Request to create a Quality on Demand session\",\n  \"type\": \"object\",\n  \"required\": [\n    \"phoneNumber\",\n    \"qosProfile\",\n    \"duration\"\n  ],\n  \"properties\": {\n    \"phoneNumber\": {\n      \"type\": \"string\"\n    },\n    \"qosProfile\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"LOW_LATENCY\",\n        \"THROUGHPUT_S\",\n        \"THROUGHPUT_M\",\n        \"THROUGHPUT_L\",\n        \"VOICE\"\n      ]\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"minimum\": 60,\n      \"maximum\": 86400\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/network-apis-create-session-request-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Create QoD Session Request
---
