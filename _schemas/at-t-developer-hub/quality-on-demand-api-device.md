---
description: Device identifier for QoD session
layout: schema
name: Device
properties_list:
- description: Mobile phone number in E.164 format
  name: phoneNumber
  type: string
- description: Device IPv4 address
  name: ipv4Address
  type: object
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/quality-on-demand-api-device-schema.json
slug: quality-on-demand-api-device
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/quality-on-demand-api-device-schema.json\",\n  \"title\": \"Device\",\n  \"description\": \"Device identifier for QoD session\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Mobile phone number in E.164 format\",\n      \"example\": \"+12125551234\"\n    },\n    \"ipv4Address\": {\n      \"type\": \"object\",\n      \"description\": \"Device IPv4 address\",\n      \"properties\": {\n        \"publicAddress\": {\n          \"type\": \"string\",\n          \"description\": \"Public IPv4 address\",\n          \"example\": \"203.0.113.42\"\n        },\n        \"privateAddress\": {\n          \"type\": \"string\",\n          \"description\": \"Private IPv4 address\",\n          \"example\": \"10.0.0.5\"\n        }\n      }\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/quality-on-demand-api-device-schema.json
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
