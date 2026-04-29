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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-flight-end-point-schema.json
slug: seat-map-display-flight-end-point
source_filename: seat-map-display-flight-end-point-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-flight-end-point-schema.json\",\n  \"title\": \"FlightEndPoint\",\n  \"description\": \"departure or arrival information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iataCode\": {\n      \"description\": \"[IATA airline codes](http://www.iata.org/publications/Pages/code-search.aspx)\",\n      \"type\": \"string\",\n      \"example\": \"JFK\"\n    },\n    \"terminal\": {\n      \"description\": \"terminal name / number\",\n      \"type\": \"string\",\n      \"example\": \"T2\"\n    },\n    \"at\": {\n      \"description\": \"local date and time in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-ddThh:mm\\u00b1hh:mm format, e.g. 2017-02-10T20:40:00+02:00\",\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2017-10-23T20:00:00+02:00\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-flight-end-point-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: FlightEndPoint
---
