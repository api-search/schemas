---
description: Current connectivity status of a device on AT&T network
layout: schema
name: Device Connectivity Status
properties_list:
- description: ''
  name: connectivityStatus
  type: string
- description: ''
  name: networkGeneration
  type: string
- description: ''
  name: roaming
  type: boolean
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/network-apis-device-connectivity-status-schema.json
slug: network-apis-device-connectivity-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.att.com/schemas/network/device-connectivity-status\",\n  \"title\": \"Device Connectivity Status\",\n  \"description\": \"Current connectivity status of a device on AT&T network\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectivityStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CONNECTED_DATA\",\n        \"CONNECTED_SMS\",\n        \"NOT_CONNECTED\"\n      ]\n    },\n    \"networkGeneration\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"5G\",\n        \"5G_NSA\",\n        \"4G\",\n        \"3G\"\n      ]\n    },\n    \"roaming\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/network-apis-device-connectivity-status-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Device Connectivity Status
---
