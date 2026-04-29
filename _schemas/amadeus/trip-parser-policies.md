---
description: Booking Rules
layout: schema
name: policies
properties_list:
- description: ''
  name: cancellation
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-policies-schema.json
slug: trip-parser-policies
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"policies\",\n  \"description\": \"Booking Rules\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cancellation\": {\n      \"$ref\": \"#/definitions/cancellation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-policies-schema.json
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
title: policies
---
