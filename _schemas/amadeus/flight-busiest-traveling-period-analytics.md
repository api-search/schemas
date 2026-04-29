---
description: ''
layout: schema
name: Analytics
properties_list:
- description: ''
  name: travelers
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-busiest-traveling-period-analytics-schema.json
slug: flight-busiest-traveling-period-analytics
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Analytics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"travelers\": {\n      \"$ref\": \"#/definitions/Travelers\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-busiest-traveling-period-analytics-schema.json
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
