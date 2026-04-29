---
description: SimSwapCheckResponse schema
layout: schema
name: SimSwapCheckResponse
properties_list:
- description: True if a SIM swap was detected within the maxAge period, false otherwise.
  name: swapped
  type: boolean
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/sim-swap-api-sim-swap-check-response-schema.json
slug: sim-swap-api-sim-swap-check-response
source_filename: sim-swap-api-sim-swap-check-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/sim-swap-api-sim-swap-check-response-schema.json\",\n  \"title\": \"SimSwapCheckResponse\",\n  \"description\": \"SimSwapCheckResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"swapped\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if a SIM swap was detected within the maxAge period, false otherwise.\",\n      \"example\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/sim-swap-api-sim-swap-check-response-schema.json
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: SimSwapCheckResponse
---
