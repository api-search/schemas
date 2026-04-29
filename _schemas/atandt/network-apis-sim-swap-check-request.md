---
description: Request to check if a SIM swap has occurred
layout: schema
name: SIM Swap Check Request
properties_list:
- description: ''
  name: phoneNumber
  type: string
- description: ''
  name: maxAge
  type: integer
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/network-apis-sim-swap-check-request-schema.json
slug: network-apis-sim-swap-check-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.att.com/schemas/network/sim-swap-check-request\",\n  \"title\": \"SIM Swap Check Request\",\n  \"description\": \"Request to check if a SIM swap has occurred\",\n  \"type\": \"object\",\n  \"required\": [\n    \"phoneNumber\"\n  ],\n  \"properties\": {\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\+[1-9]\\\\d{1,14}$\"\n    },\n    \"maxAge\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 2400\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/network-apis-sim-swap-check-request-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: SIM Swap Check Request
---
