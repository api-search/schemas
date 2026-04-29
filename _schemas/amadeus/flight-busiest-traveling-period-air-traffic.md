---
description: ''
layout: schema
name: Air_Traffic
properties_list:
- description: ''
  name: type
  type: string
- description: Time period following [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) standard
  name: period
  type: string
- description: ''
  name: analytics
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-busiest-traveling-period-air-traffic-schema.json
slug: flight-busiest-traveling-period-air-traffic
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Air_Traffic\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"period\": {\n      \"type\": \"string\",\n      \"description\": \"Time period following [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) standard\"\n    },\n    \"analytics\": {\n      \"$ref\": \"#/definitions/Analytics\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-busiest-traveling-period-air-traffic-schema.json
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
title: Air_Traffic
---
