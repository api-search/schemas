---
description: CreateSessionRequest schema
layout: schema
name: CreateSessionRequest
properties_list:
- description: Device identifier for QoD session
  name: device
  type: object
- description: Requested QoS profile
  name: qosProfile
  type: string
- description: Session duration in seconds (default and max vary by profile)
  name: duration
  type: integer
- description: Webhook URL to receive QoS status change notifications
  name: notificationUrl
  type: string
- description: Bearer token for webhook notification authentication
  name: notificationAuthToken
  type: string
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/quality-on-demand-api-create-session-request-schema.json
slug: quality-on-demand-api-create-session-request
source_filename: quality-on-demand-api-create-session-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/quality-on-demand-api-create-session-request-schema.json\",\n  \"title\": \"CreateSessionRequest\",\n  \"description\": \"CreateSessionRequest schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"device\",\n    \"qosProfile\"\n  ],\n  \"properties\": {\n    \"device\": {\n      \"type\": \"object\",\n      \"description\": \"Device identifier for QoD session\",\n      \"properties\": {\n        \"phoneNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Mobile phone number in E.164 format\",\n          \"example\": \"+12125551234\"\n        },\n        \"ipv4Address\": {\n          \"type\": \"object\",\n          \"description\": \"Device IPv4 address\",\n          \"properties\": {\n            \"publicAddress\": {\n              \"type\": \"string\",\n              \"\
  description\": \"Public IPv4 address\",\n              \"example\": \"203.0.113.42\"\n            },\n            \"privateAddress\": {\n              \"type\": \"string\",\n              \"description\": \"Private IPv4 address\",\n              \"example\": \"10.0.0.5\"\n            }\n          }\n        }\n      }\n    },\n    \"qosProfile\": {\n      \"type\": \"string\",\n      \"description\": \"Requested QoS profile\",\n      \"enum\": [\n        \"LOW_LATENCY\",\n        \"THROUGHPUT_S\",\n        \"THROUGHPUT_M\",\n        \"THROUGHPUT_L\",\n        \"VOICE\"\n      ],\n      \"example\": \"LOW_LATENCY\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Session duration in seconds (default and max vary by profile)\",\n      \"minimum\": 1,\n      \"maximum\": 86400,\n      \"example\": 3600\n    },\n    \"notificationUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Webhook URL to receive QoS status\
  \ change notifications\",\n      \"example\": \"https://webhook.example.com/qod-events\"\n    },\n    \"notificationAuthToken\": {\n      \"type\": \"string\",\n      \"description\": \"Bearer token for webhook notification authentication\",\n      \"example\": \"webhook-token-abc123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/quality-on-demand-api-create-session-request-schema.json
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: CreateSessionRequest
---
