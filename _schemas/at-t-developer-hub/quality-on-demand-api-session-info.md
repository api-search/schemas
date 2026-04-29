---
description: SessionInfo schema
layout: schema
name: SessionInfo
properties_list:
- description: Unique identifier for the QoD session
  name: sessionId
  type: string
- description: Device identifier for QoD session
  name: device
  type: object
- description: QoS profile applied to this session
  name: qosProfile
  type: string
- description: Session duration in seconds
  name: duration
  type: integer
- description: Session start timestamp
  name: startedAt
  type: string
- description: Session expiry timestamp
  name: expiresAt
  type: string
- description: Current QoS provisioning status
  name: qosStatus
  type: string
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/quality-on-demand-api-session-info-schema.json
slug: quality-on-demand-api-session-info
source_filename: quality-on-demand-api-session-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/quality-on-demand-api-session-info-schema.json\",\n  \"title\": \"SessionInfo\",\n  \"description\": \"SessionInfo schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the QoD session\",\n      \"example\": \"session-a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"device\": {\n      \"type\": \"object\",\n      \"description\": \"Device identifier for QoD session\",\n      \"properties\": {\n        \"phoneNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Mobile phone number in E.164 format\",\n          \"example\": \"+12125551234\"\n        },\n        \"ipv4Address\": {\n          \"type\": \"object\",\n          \"description\": \"Device IPv4 address\",\n         \
  \ \"properties\": {\n            \"publicAddress\": {\n              \"type\": \"string\",\n              \"description\": \"Public IPv4 address\",\n              \"example\": \"203.0.113.42\"\n            },\n            \"privateAddress\": {\n              \"type\": \"string\",\n              \"description\": \"Private IPv4 address\",\n              \"example\": \"10.0.0.5\"\n            }\n          }\n        }\n      }\n    },\n    \"qosProfile\": {\n      \"type\": \"string\",\n      \"description\": \"QoS profile applied to this session\",\n      \"enum\": [\n        \"LOW_LATENCY\",\n        \"THROUGHPUT_S\",\n        \"THROUGHPUT_M\",\n        \"THROUGHPUT_L\",\n        \"VOICE\"\n      ],\n      \"example\": \"LOW_LATENCY\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Session duration in seconds\",\n      \"example\": 3600\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Session start timestamp\",\n      \"example\": \"2026-04-19T14:30:00Z\"\n    },\n    \"expiresAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Session expiry timestamp\",\n      \"example\": \"2026-04-19T15:30:00Z\"\n    },\n    \"qosStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current QoS provisioning status\",\n      \"enum\": [\n        \"REQUESTED\",\n        \"AVAILABLE\",\n        \"UNAVAILABLE\"\n      ],\n      \"example\": \"AVAILABLE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/quality-on-demand-api-session-info-schema.json
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: SessionInfo
---
