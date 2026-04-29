---
description: ''
layout: schema
name: Delay
properties_list:
- description: the delay recorded for the timing following [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601#Durations)
  name: duration
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/on-demand-flight-status-delay-schema.json
slug: on-demand-flight-status-delay
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Delay\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"the delay recorded for the timing following [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601#Durations)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/on-demand-flight-status-delay-schema.json
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
title: Delay
---
