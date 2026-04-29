---
description: seat map information
layout: schema
name: SeatMap
properties_list:
- description: Ressource name
  name: type
  type: string
- description: item identifier
  name: id
  type: string
- description: ''
  name: self
  type: object
- description: ''
  name: departure
  type: object
- description: ''
  name: arrival
  type: object
- description: providing the marketing airline carrier code
  name: carrierCode
  type: string
- description: the flight number as assigned by the marketing carrier
  name: number
  type: string
- description: ''
  name: operating
  type: object
- description: ''
  name: aircraft
  type: object
- description: reservation booking designator (RBD) of the carrier
  name: class
  type: string
- description: Id of the impacted flight offer
  name: flightOfferId
  type: string
- description: Id of the impacted segment
  name: segmentId
  type: string
- description: decks information
  name: decks
  type: array
- description: ''
  name: aircraftCabinAmenities
  type: object
- description: number of seats available for each passenger
  name: availableSeatsCounters
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-seatmap-schema.json
slug: seatmap-display-seatmap
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"SeatMap\",\n  \"description\": \"seat map information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Ressource name\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"item identifier\"\n    },\n    \"self\": {\n      \"$ref\": \"#/definitions/Link\"\n    },\n    \"departure\": {\n      \"$ref\": \"#/definitions/FlightEndPoint\"\n    },\n    \"arrival\": {\n      \"$ref\": \"#/definitions/FlightEndPoint\"\n    },\n    \"carrierCode\": {\n      \"type\": \"string\",\n      \"description\": \"providing the marketing airline carrier code\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"the flight number as assigned by the marketing carrier\"\n    },\n    \"operating\": {\n      \"$ref\": \"#/definitions/OperatingFlight\"\n    },\n    \"aircraft\": {\n      \"$ref\"\
  : \"#/definitions/AircraftEquipment\"\n    },\n    \"class\": {\n      \"type\": \"string\",\n      \"description\": \"reservation booking designator (RBD) of the carrier\"\n    },\n    \"flightOfferId\": {\n      \"type\": \"string\",\n      \"description\": \"Id of the impacted flight offer\"\n    },\n    \"segmentId\": {\n      \"type\": \"string\",\n      \"description\": \"Id of the impacted segment\"\n    },\n    \"decks\": {\n      \"type\": \"array\",\n      \"description\": \"decks information\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Deck\"\n      }\n    },\n    \"aircraftCabinAmenities\": {\n      \"$ref\": \"#/definitions/AircraftCabinAmenities\"\n    },\n    \"availableSeatsCounters\": {\n      \"type\": \"array\",\n      \"description\": \"number of seats available for each passenger\",\n      \"items\": {\n        \"$ref\": \"#/definitions/AvailableSeatsCounter\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-seatmap-schema.json
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
title: SeatMap
---
