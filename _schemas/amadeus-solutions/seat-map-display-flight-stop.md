---
description: details of stops for direct or change of gauge flights
layout: schema
name: FlightStop
properties_list:
- description: '[IATA airline codes](http://www.iata.org/publications/Pages/code-search.aspx)'
  name: iataCode
  type: string
- description: ''
  name: newAircraft
  type: object
- description: stop duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M
  name: duration
  type: string
- description: arrival at the stop in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-ddThh:mm±hh:mm format, e.g. 2017-02-10T20:40:00+02:00
  name: arrivalAt
  type: string
- description: departure from the stop in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-ddThh:mm±hh:mm format, e.g. 2017-02-10T20:40:00+02:00
  name: departureAt
  type: string
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-flight-stop-schema.json
slug: seat-map-display-flight-stop
source_filename: seat-map-display-flight-stop-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-flight-stop-schema.json\",\n  \"title\": \"FlightStop\",\n  \"description\": \"details of stops for direct or change of gauge flights\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iataCode\": {\n      \"description\": \"[IATA airline codes](http://www.iata.org/publications/Pages/code-search.aspx)\",\n      \"type\": \"string\",\n      \"example\": \"JFK\"\n    },\n    \"newAircraft\": {\n      \"$ref\": \"#/definitions/AircraftEquipment\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"stop duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M\",\n      \"example\": \"PT2H10M\"\n    },\n    \"arrivalAt\": {\n      \"description\": \"arrival at the stop in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601)\
  \ YYYY-MM-ddThh:mm\\u00b1hh:mm format, e.g. 2017-02-10T20:40:00+02:00\",\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2017-10-23T20:00:00+02:00\"\n    },\n    \"departureAt\": {\n      \"description\": \"departure from the stop in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-ddThh:mm\\u00b1hh:mm format, e.g. 2017-02-10T20:40:00+02:00\",\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2017-10-23T20:00:00+02:00\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-flight-stop-schema.json
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
