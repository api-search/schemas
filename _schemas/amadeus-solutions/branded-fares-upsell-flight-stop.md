---
description: details of stops for direct or change of gauge flights
layout: schema
name: FlightStop
properties_list: []
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/branded-fares-upsell-flight-stop-schema.json
slug: branded-fares-upsell-flight-stop
source_filename: branded-fares-upsell-flight-stop-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-flight-stop-schema.json\",\n  \"title\": \"FlightStop\",\n  \"description\": \"details of stops for direct or change of gauge flights\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/OriginalFlightStop\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"arrivalAt\": {\n          \"description\": \"arrival at the stop in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-ddThh:mm:ss format, e.g. 2017-02-10T20:40:00\",\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"example\": \"2017-10-23T20:00:00\"\n        },\n        \"departureAt\": {\n          \"description\": \"departure from the stop in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-ddThh:mm:ss format, e.g. 2017-02-10T20:40:00\",\n\
  \          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"example\": \"2017-10-23T20:00:00\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-flight-stop-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: FlightStop
---
