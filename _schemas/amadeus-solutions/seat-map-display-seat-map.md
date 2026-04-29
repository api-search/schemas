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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-seat-map-schema.json
slug: seat-map-display-seat-map
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-seat-map-schema.json\",\n  \"title\": \"SeatMap\",\n  \"description\": \"seat map information\",\n  \"properties\": {\n    \"type\": {\n      \"description\": \"Ressource name\",\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"example\": \"seatmap\"\n    },\n    \"id\": {\n      \"description\": \"item identifier\",\n      \"type\": \"string\"\n    },\n    \"self\": {\n      \"$ref\": \"#/definitions/Link\"\n    },\n    \"departure\": {\n      \"$ref\": \"#/definitions/FlightEndPoint\"\n    },\n    \"arrival\": {\n      \"$ref\": \"#/definitions/FlightEndPoint\"\n    },\n    \"carrierCode\": {\n      \"type\": \"string\",\n      \"description\": \"providing the marketing airline carrier code\",\n      \"minLength\": 1,\n      \"maxLength\": 2,\n      \"example\": \"\
  DL\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"the flight number as assigned by the marketing carrier\",\n      \"minLength\": 1,\n      \"maxLength\": 4,\n      \"example\": \"212\"\n    },\n    \"operating\": {\n      \"$ref\": \"#/definitions/OperatingFlight\"\n    },\n    \"aircraft\": {\n      \"$ref\": \"#/definitions/AircraftEquipment\"\n    },\n    \"class\": {\n      \"type\": \"string\",\n      \"description\": \"reservation booking designator (RBD) of the carrier\",\n      \"minLength\": 1,\n      \"maxLength\": 2\n    },\n    \"flightOfferId\": {\n      \"description\": \"Id of the impacted flight offer\",\n      \"type\": \"string\",\n      \"example\": \"1\"\n    },\n    \"segmentId\": {\n      \"description\": \"Id of the impacted segment\",\n      \"type\": \"string\",\n      \"example\": \"1\"\n    },\n    \"decks\": {\n      \"type\": \"array\",\n      \"description\": \"decks information\",\n      \"items\": {\n        \"$ref\"\
  : \"#/definitions/Deck\"\n      }\n    },\n    \"aircraftCabinAmenities\": {\n      \"$ref\": \"#/definitions/AircraftCabinAmenities\"\n    },\n    \"availableSeatsCounters\": {\n      \"type\": \"array\",\n      \"description\": \"number of seats available for each passenger\",\n      \"items\": {\n        \"$ref\": \"#/definitions/AvailableSeatsCounter\"\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-seat-map-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: SeatMap
---
