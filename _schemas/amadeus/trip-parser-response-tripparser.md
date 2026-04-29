---
description: ''
layout: schema
name: response_tripParser
properties_list:
- description: ''
  name: data
  type: object
- description: ''
  name: warnings
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-response-tripparser-schema.json
slug: trip-parser-response-tripparser
source_filename: trip-parser-response-tripparser-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"response_tripParser\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"$ref\": \"#/definitions/trip\"\n    },\n    \"warnings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/warnings\"\n      }\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-response-tripparser-schema.json
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
title: response_tripParser
---
