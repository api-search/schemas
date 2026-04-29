---
description: ''
layout: schema
name: Gate
properties_list:
- description: the main gate number
  name: mainGate
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/on-demand-flight-status-gate-schema.json
slug: on-demand-flight-status-gate
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Gate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mainGate\": {\n      \"type\": \"string\",\n      \"description\": \"the main gate number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/on-demand-flight-status-gate-schema.json
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: Gate
---
