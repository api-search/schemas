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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-flightstop-schema.json
slug: seatmap-display-flightstop
source_filename: seatmap-display-flightstop-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FlightStop\",\n  \"description\": \"details of stops for direct or change of gauge flights\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iataCode\": {\n      \"type\": \"string\",\n      \"description\": \"[IATA airline codes](http://www.iata.org/publications/Pages/code-search.aspx)\"\n    },\n    \"newAircraft\": {\n      \"$ref\": \"#/definitions/AircraftEquipment\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"stop duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M\"\n    },\n    \"arrivalAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"arrival at the stop in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-ddThh:mm\\u00b1hh:mm format, e.g. 2017-02-10T20:40:00+02:00\"\n    },\n    \"departureAt\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"departure from the stop in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-ddThh:mm\\u00b1hh:mm format, e.g. 2017-02-10T20:40:00+02:00\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-flightstop-schema.json
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
title: FlightStop
---
