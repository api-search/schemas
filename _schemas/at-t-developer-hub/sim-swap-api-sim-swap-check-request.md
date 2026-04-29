---
description: SimSwapCheckRequest schema
layout: schema
name: SimSwapCheckRequest
properties_list:
- description: Mobile phone number in E.164 format associated with the SIM to check.
  name: phoneNumber
  type: string
- description: Maximum age in hours to check for a SIM swap. If not provided, the default lookback period is used.
  name: maxAge
  type: integer
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/sim-swap-api-sim-swap-check-request-schema.json
slug: sim-swap-api-sim-swap-check-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/sim-swap-api-sim-swap-check-request-schema.json\",\n  \"title\": \"SimSwapCheckRequest\",\n  \"description\": \"SimSwapCheckRequest schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"phoneNumber\"\n  ],\n  \"properties\": {\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Mobile phone number in E.164 format associated with the SIM to check.\",\n      \"example\": \"+12125551234\"\n    },\n    \"maxAge\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum age in hours to check for a SIM swap. If not provided, the default lookback period is used.\",\n      \"minimum\": 1,\n      \"maximum\": 2400,\n      \"example\": 240\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/sim-swap-api-sim-swap-check-request-schema.json
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: SimSwapCheckRequest
---
