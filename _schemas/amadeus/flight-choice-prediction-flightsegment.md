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
- description: the flight number suffix as assigned by the carrier
  name: suffix
  type: string
- description: ''
  name: aircraft
  type: object
- description: reservation booking designator (RBD) of the carrier
  name: class
  type: string
- description: booking cabin / class of service of the carrier
  name: cabin
  type: string
- description: ''
  name: operating
  type: object
- description: stop duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M
  name: duration
  type: string
- description: information regarding the different stops composing the flight segment. E.g. technical stop, change of gauge...
  name: stops
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-choice-prediction-flightsegment-schema.json
slug: flight-choice-prediction-flightsegment
source_filename: flight-choice-prediction-flightsegment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FlightSegment\",\n  \"description\": \"defining a flight segment; including both operating and marketing details when applicable\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"departure\": {\n      \"$ref\": \"#/definitions/FlightEndPoint\"\n    },\n    \"arrival\": {\n      \"$ref\": \"#/definitions/FlightEndPoint\"\n    },\n    \"carrierCode\": {\n      \"type\": \"string\",\n      \"description\": \"providing the airline / carrier code\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"the flight number as assigned by the carrier\"\n    },\n    \"suffix\": {\n      \"type\": \"string\",\n      \"description\": \"the flight number suffix as assigned by the carrier\"\n    },\n    \"aircraft\": {\n      \"$ref\": \"#/definitions/AircraftEquipment\"\n    },\n    \"class\": {\n      \"type\": \"string\",\n      \"description\": \"reservation booking designator\
  \ (RBD) of the carrier\"\n    },\n    \"cabin\": {\n      \"type\": \"string\",\n      \"description\": \"booking cabin / class of service of the carrier\"\n    },\n    \"operating\": {\n      \"$ref\": \"#/definitions/OperatingFlight\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"stop duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M\"\n    },\n    \"stops\": {\n      \"type\": \"array\",\n      \"description\": \"information regarding the different stops composing the flight segment. E.g. technical stop, change of gauge...\",\n      \"items\": {\n        \"$ref\": \"#/definitions/FlightStop\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-choice-prediction-flightsegment-schema.json
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
title: FlightSegment
---
