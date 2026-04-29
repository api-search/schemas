---
description: ''
layout: schema
name: FlightAvailability
properties_list:
- description: the resource name
  name: type
  type: string
- description: Id of the flight availability
  name: id
  type: string
- description: Id of the originDestination in query
  name: originDestinationId
  type: string
- description: ''
  name: source
  type: object
- description: If true, inform that a ticketing will be required at booking step.
  name: instantTicketingRequired
  type: boolean
- description: If true, a payment card is mandatory to book this flight offer
  name: paymentCardRequired
  type: boolean
- description: duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M for a duration of 2h10m
  name: duration
  type: string
- description: ''
  name: segments
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-availibilities-search-flightavailability-schema.json
slug: flight-availibilities-search-flightavailability
source_filename: flight-availibilities-search-flightavailability-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FlightAvailability\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"the resource name\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Id of the flight availability\"\n    },\n    \"originDestinationId\": {\n      \"type\": \"string\",\n      \"description\": \"Id of the originDestination in query\"\n    },\n    \"source\": {\n      \"$ref\": \"#/definitions/FlightOfferSource\"\n    },\n    \"instantTicketingRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, inform that a ticketing will be required at booking step.\"\n    },\n    \"paymentCardRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, a payment card is mandatory to book this flight offer\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"duration in\
  \ [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M for a duration of 2h10m\"\n    },\n    \"segments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Extended_Segment\"\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"id\",\n    \"source\",\n    \"segments\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-availibilities-search-flightavailability-schema.json
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
title: FlightAvailability
---
