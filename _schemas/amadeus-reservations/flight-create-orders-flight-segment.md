---
description: defining a flight segment; including both operating and marketing details when applicable
layout: schema
name: FlightSegment
properties_list:
- description: ''
  name: departure
  type: object
- description: ''
  name: arrival
  type: object
- description: providing the airline / carrier code
  name: carrierCode
  type: string
- description: the flight number as assigned by the carrier
  name: number
  type: string
- description: ''
  name: aircraft
  type: object
- description: ''
  name: operating
  type: object
- description: stop duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M
  name: duration
  type: string
- description: information regarding the different stops composing the flight segment. E.g. technical stop, change of gauge...
  name: stops
  type: array
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-flight-segment-schema.json
slug: flight-create-orders-flight-segment
source_filename: flight-create-orders-flight-segment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-flight-segment-schema.json\",\n  \"title\": \"FlightSegment\",\n  \"description\": \"defining a flight segment; including both operating and marketing details when applicable\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"departure\": {\n      \"$ref\": \"#/definitions/FlightEndPoint\"\n    },\n    \"arrival\": {\n      \"$ref\": \"#/definitions/FlightEndPoint\"\n    },\n    \"carrierCode\": {\n      \"type\": \"string\",\n      \"description\": \"providing the airline / carrier code\",\n      \"minLength\": 1,\n      \"maxLength\": 2,\n      \"example\": \"DL\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"the flight number as assigned by the carrier\",\n      \"minLength\": 1,\n      \"maxLength\": 4,\n      \"example\": \"212\"\n\
  \    },\n    \"aircraft\": {\n      \"$ref\": \"#/definitions/AircraftEquipment\"\n    },\n    \"operating\": {\n      \"$ref\": \"#/definitions/OperatingFlight\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"stop duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M\",\n      \"example\": \"PT2H10M\"\n    },\n    \"stops\": {\n      \"type\": \"array\",\n      \"description\": \"information regarding the different stops composing the flight segment. E.g. technical stop, change of gauge...\",\n      \"items\": {\n        \"$ref\": \"#/definitions/FlightStop\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-flight-segment-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: FlightSegment
---
