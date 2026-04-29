---
description: An object representing weight and unit.
layout: schema
name: weight
properties_list:
- description: Defines the weight value with the specified unit with decimal position.
  name: amount
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-weight-schema.json
slug: trip-parser-weight
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"weight\",\n  \"description\": \"An object representing weight and unit.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"string\",\n      \"description\": \"Defines the weight value with the specified unit with decimal position.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-weight-schema.json
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
title: weight
---
