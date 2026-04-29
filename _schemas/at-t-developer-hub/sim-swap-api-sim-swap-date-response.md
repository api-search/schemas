---
description: SimSwapDateResponse schema
layout: schema
name: SimSwapDateResponse
properties_list:
- description: Date and time of the most recent SIM swap, or null if no swap has been detected recently.
  name: latestSimChange
  type: string
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/sim-swap-api-sim-swap-date-response-schema.json
slug: sim-swap-api-sim-swap-date-response
source_filename: sim-swap-api-sim-swap-date-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/sim-swap-api-sim-swap-date-response-schema.json\",\n  \"title\": \"SimSwapDateResponse\",\n  \"description\": \"SimSwapDateResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"latestSimChange\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"Date and time of the most recent SIM swap, or null if no swap has been detected recently.\",\n      \"example\": null\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/sim-swap-api-sim-swap-date-response-schema.json
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: SimSwapDateResponse
---
