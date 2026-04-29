---
description: ''
layout: schema
name: trip
properties_list:
- description: the resource name
  name: type
  type: string
- description: Reference of the Trip
  name: reference
  type: string
- description: Date of the trip point optional time and time offset in ISO 8601 format, e.g. 2017-02-10T20:40:00+02:00
  name: creationDateTime
  type: string
- description: itinerary booking date
  name: bookingDate
  type: string
- description: Ticket No(Specially for Air and Train segment)
  name: bookingNumber
  type: string
- description: information of the booking provider
  name: provider
  type: string
- description: Trip label or name
  name: title
  type: string
- description: Trip description
  name: description
  type: string
- description: ''
  name: start
  type: object
- description: ''
  name: end
  type: object
- description: ''
  name: travelAgency
  type: object
- description: ''
  name: stakeholders
  type: array
- description: ''
  name: price
  type: object
- description: ''
  name: products
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-trip-schema.json
slug: trip-parser-trip
source_filename: trip-parser-trip-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"trip\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"the resource name\"\n    },\n    \"reference\": {\n      \"type\": \"string\",\n      \"description\": \"Reference of the Trip\"\n    },\n    \"creationDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the trip point optional time and time offset in ISO 8601 format, e.g. 2017-02-10T20:40:00+02:00\"\n    },\n    \"bookingDate\": {\n      \"type\": \"string\",\n      \"description\": \"itinerary booking date\"\n    },\n    \"bookingNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Ticket No(Specially for Air and Train segment)\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"information of the booking provider\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Trip\
  \ label or name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Trip description\"\n    },\n    \"start\": {\n      \"$ref\": \"#/definitions/start\"\n    },\n    \"end\": {\n      \"$ref\": \"#/definitions/end\"\n    },\n    \"travelAgency\": {\n      \"$ref\": \"#/definitions/travelAgency\"\n    },\n    \"stakeholders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/stakeholder\"\n      }\n    },\n    \"price\": {\n      \"$ref\": \"#/definitions/price\"\n    },\n    \"products\": {\n      \"type\": \"array\",\n      \"items\": {}\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-trip-schema.json
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
title: trip
---
