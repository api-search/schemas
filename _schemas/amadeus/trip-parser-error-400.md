---
description: ''
layout: schema
name: error_400
properties_list:
- description: ''
  name: errors
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-error-400-schema.json
slug: trip-parser-error-400
source_filename: trip-parser-error-400-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"error_400\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/issue\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-error-400-schema.json
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
title: error_400
---
