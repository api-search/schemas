---
description: ''
layout: schema
name: Error_401
properties_list:
- description: ''
  name: errors
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-error-401-schema.json
slug: transfer-booking-error-401
source_filename: transfer-booking-error-401-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Error_401\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Issue\"\n      }\n    }\n  },\n  \"required\": [\n    \"errors\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-booking-error-401-schema.json
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
title: Error_401
---
