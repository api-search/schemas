---
description: ''
layout: schema
name: meal
properties_list:
- description: Code of the meal served on board
  name: code
  type: string
- description: Description of the meal served on board
  name: description
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-meal-schema.json
slug: trip-parser-meal
source_filename: trip-parser-meal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"meal\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Code of the meal served on board\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the meal served on board\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-meal-schema.json
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
title: meal
---
