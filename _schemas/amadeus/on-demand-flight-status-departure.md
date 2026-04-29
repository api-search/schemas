---
description: ''
layout: schema
name: Departure
properties_list:
- description: ''
  name: terminal
  type: object
- description: ''
  name: gate
  type: object
- description: the list of timings
  name: timings
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/on-demand-flight-status-departure-schema.json
slug: on-demand-flight-status-departure
source_filename: on-demand-flight-status-departure-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Departure\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"terminal\": {\n      \"$ref\": \"#/definitions/Terminal\"\n    },\n    \"gate\": {\n      \"$ref\": \"#/definitions/Gate\"\n    },\n    \"timings\": {\n      \"type\": \"array\",\n      \"description\": \"the list of timings\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Timing\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/on-demand-flight-status-departure-schema.json
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
title: Departure
---
