---
description: Roaming status and location information for a device
layout: schema
name: Device Roaming Status
properties_list:
- description: ''
  name: roaming
  type: boolean
- description: ''
  name: countryCode
  type: string
- description: ''
  name: countryName
  type: string
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/network-apis-device-roaming-status-schema.json
slug: network-apis-device-roaming-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.att.com/schemas/network/device-roaming-status\",\n  \"title\": \"Device Roaming Status\",\n  \"description\": \"Roaming status and location information for a device\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roaming\": {\n      \"type\": \"boolean\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\"\n    },\n    \"countryName\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/network-apis-device-roaming-status-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Device Roaming Status
---
