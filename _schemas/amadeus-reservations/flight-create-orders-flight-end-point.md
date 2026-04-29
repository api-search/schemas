---
description: departure or arrival information
layout: schema
name: FlightEndPoint
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-flight-end-point-schema.json
slug: flight-create-orders-flight-end-point
source_filename: flight-create-orders-flight-end-point-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-flight-end-point-schema.json\",\n  \"title\": \"FlightEndPoint\",\n  \"description\": \"departure or arrival information\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/OriginalFlightEndPoint\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"at\": {\n          \"description\": \"local date and time in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-ddThh:mm:ss format, e.g. 2017-02-10T20:40:00\",\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"example\": \"2017-10-23T20:00:00\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-flight-end-point-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: FlightEndPoint
---
