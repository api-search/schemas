---
description: ''
layout: schema
name: Timing
properties_list:
- description: the qualifier of the timing. e.g. STD (stands for Schedule Time Departure)
  name: qualifier
  type: string
- description: ''
  name: value
  type: string
- description: delays that might be recorded on a timing
  name: delays
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/on-demand-flight-status-timing-schema.json
slug: on-demand-flight-status-timing
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Timing\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"qualifier\": {\n      \"type\": \"string\",\n      \"description\": \"the qualifier of the timing. e.g. STD (stands for Schedule Time Departure)\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"delays\": {\n      \"type\": \"array\",\n      \"description\": \"delays that might be recorded on a timing\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Delay\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/on-demand-flight-status-timing-schema.json
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
title: Timing
---
