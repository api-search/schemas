---
description: ''
layout: schema
name: driver
properties_list:
- description: ''
  name: contacts
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-driver-schema.json
slug: trip-parser-driver
source_filename: trip-parser-driver-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"driver\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contacts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/contact\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-driver-schema.json
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
title: driver
---
