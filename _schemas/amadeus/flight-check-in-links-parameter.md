---
description: ''
layout: schema
name: Parameter
properties_list:
- description: parameter descriptive information
  name: description
  type: string
- description: type of the parameter
  name: type
  type: string
- description: format of the parameter
  name: format
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-check-in-links-parameter-schema.json
slug: flight-check-in-links-parameter
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Parameter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"parameter descriptive information\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"type of the parameter\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"format of the parameter\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-check-in-links-parameter-schema.json
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
title: Parameter
---
