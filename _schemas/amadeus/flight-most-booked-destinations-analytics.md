---
description: ''
layout: schema
name: Analytics
properties_list:
- description: ''
  name: flights
  type: object
- description: ''
  name: travelers
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-most-booked-destinations-analytics-schema.json
slug: flight-most-booked-destinations-analytics
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Analytics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flights\": {\n      \"$ref\": \"#/definitions/Flights\"\n    },\n    \"travelers\": {\n      \"$ref\": \"#/definitions/Travelers\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-most-booked-destinations-analytics-schema.json
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
title: Analytics
---
