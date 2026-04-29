---
description: Device identifier for network metrics queries
layout: schema
name: Device
properties_list:
- description: Mobile phone number in E.164 format
  name: phoneNumber
  type: string
- description: Device IP address (alternative to phoneNumber)
  name: ipv4Address
  type: object
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/network-insights-api-device-schema.json
slug: network-insights-api-device
source_filename: network-insights-api-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/network-insights-api-device-schema.json\",\n  \"title\": \"Device\",\n  \"description\": \"Device identifier for network metrics queries\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Mobile phone number in E.164 format\",\n      \"example\": \"+12125551234\"\n    },\n    \"ipv4Address\": {\n      \"type\": \"object\",\n      \"description\": \"Device IP address (alternative to phoneNumber)\",\n      \"properties\": {\n        \"publicAddress\": {\n          \"type\": \"string\",\n          \"example\": \"203.0.113.42\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/network-insights-api-device-schema.json
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: Device
---
