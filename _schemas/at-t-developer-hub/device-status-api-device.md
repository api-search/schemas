---
description: Device identifier for connectivity status queries
layout: schema
name: Device
properties_list:
- description: Mobile phone number in E.164 format
  name: phoneNumber
  type: string
- description: Device IPv4 address (alternative to phoneNumber)
  name: ipv4Address
  type: object
- description: Network access identifier (alternative to phoneNumber)
  name: networkAccessIdentifier
  type: string
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/device-status-api-device-schema.json
slug: device-status-api-device
source_filename: device-status-api-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/device-status-api-device-schema.json\",\n  \"title\": \"Device\",\n  \"description\": \"Device identifier for connectivity status queries\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Mobile phone number in E.164 format\",\n      \"example\": \"+12125551234\"\n    },\n    \"ipv4Address\": {\n      \"type\": \"object\",\n      \"description\": \"Device IPv4 address (alternative to phoneNumber)\",\n      \"properties\": {\n        \"publicAddress\": {\n          \"type\": \"string\",\n          \"description\": \"Public IPv4 address\",\n          \"example\": \"203.0.113.42\"\n        },\n        \"privateAddress\": {\n          \"type\": \"string\",\n          \"description\": \"Private IPv4 address\",\n          \"example\"\
  : \"10.0.0.5\"\n        },\n        \"publicPort\": {\n          \"type\": \"integer\",\n          \"description\": \"Public port if behind NAT\",\n          \"example\": 54321\n        }\n      }\n    },\n    \"networkAccessIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"Network access identifier (alternative to phoneNumber)\",\n      \"example\": \"user@example.com\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/device-status-api-device-schema.json
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
