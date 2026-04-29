---
description: Alert schema from Palo Alto Networks IoT Security API
layout: schema
name: Alert
properties_list:
- description: Unique alert identifier.
  name: id
  type: string
- description: Alert type classification.
  name: type
  type: string
- description: Alert severity level.
  name: severity
  type: string
- description: Human-readable alert description.
  name: description
  type: string
- description: Identifier of the affected device.
  name: deviceid
  type: string
- description: IP address of the affected device.
  name: device_ip
  type: string
- description: Profile of the affected device.
  name: device_profile
  type: string
- description: Whether the alert has been resolved.
  name: resolved
  type: string
- description: Resolution reason if resolved.
  name: resolved_reason
  type: string
- description: Timestamp when the alert was generated.
  name: timestamp
  type: string
- description: Additional alert-specific details.
  name: details
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/iot-security-api-alert-schema.json
slug: iot-security-api-alert
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Alert\",\n  \"description\": \"Alert schema from Palo Alto Networks IoT Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/iot-security-api-alert-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique alert identifier.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Alert type classification.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\",\n        \"info\"\n      ],\n      \"description\": \"Alert severity level.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable alert description.\"\n    },\n    \"deviceid\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Identifier of the affected device.\"\n    },\n    \"device_ip\": {\n      \"type\": \"string\",\n      \"format\": \"ipv4\",\n      \"description\": \"IP address of the affected device.\"\n    },\n    \"device_profile\": {\n      \"type\": \"string\",\n      \"description\": \"Profile of the affected device.\"\n    },\n    \"resolved\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"yes\",\n        \"no\"\n      ],\n      \"description\": \"Whether the alert has been resolved.\"\n    },\n    \"resolved_reason\": {\n      \"type\": \"string\",\n      \"description\": \"Resolution reason if resolved.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the alert was generated.\"\n    },\n    \"details\": {\n      \"type\": \"object\",\n      \"description\": \"Additional alert-specific details.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/iot-security-api-alert-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Alert
---
