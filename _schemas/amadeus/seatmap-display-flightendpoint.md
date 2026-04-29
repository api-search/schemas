---
description: departure or arrival information
layout: schema
name: FlightEndPoint
properties_list:
- description: '[IATA airline codes](http://www.iata.org/publications/Pages/code-search.aspx)'
  name: iataCode
  type: string
- description: terminal name / number
  name: terminal
  type: string
- description: local date and time in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-ddThh:mm±hh:mm format, e.g. 2017-02-10T20:40:00+02:00
  name: at
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-flightendpoint-schema.json
slug: seatmap-display-flightendpoint
source_filename: seatmap-display-flightendpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FlightEndPoint\",\n  \"description\": \"departure or arrival information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iataCode\": {\n      \"type\": \"string\",\n      \"description\": \"[IATA airline codes](http://www.iata.org/publications/Pages/code-search.aspx)\"\n    },\n    \"terminal\": {\n      \"type\": \"string\",\n      \"description\": \"terminal name / number\"\n    },\n    \"at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"local date and time in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-ddThh:mm\\u00b1hh:mm format, e.g. 2017-02-10T20:40:00+02:00\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-flightendpoint-schema.json
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
title: FlightEndPoint
---
