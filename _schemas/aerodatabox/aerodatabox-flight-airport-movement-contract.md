---
description: Flight arrival or departure information
layout: schema
name: FlightAirportMovementContract
properties_list:
- description: ''
  name: airport
  type: object
- description: ''
  name: scheduledTime
  type: object
- description: ''
  name: revisedTime
  type: object
- description: ''
  name: predictedTime
  type: object
- description: ''
  name: runwayTime
  type: object
- description: Terminal of the flight
  name: terminal
  type: string
- description: Check-in desk(s) for the flight (only for departing flights)
  name: checkInDesk
  type: string
- description: Gate of (un)boarding for the flight
  name: gate
  type: string
- description: Baggage belt(s) for the flight (only for arriving flights)
  name: baggageBelt
  type: string
- description: Name of a runway of landing (for arriving flights) or take-off (for departing flights), if known.
  name: runway
  type: string
- description: Array of quality characteristics of the data. Check this to know which information you can expect within this contract (basic, live and/or approximate data).
  name: quality
  type: array
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-flight-airport-movement-contract-schema.json
slug: aerodatabox-flight-airport-movement-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-airport-movement-contract-schema.json\",\n  \"title\": \"FlightAirportMovementContract\",\n  \"description\": \"Flight arrival or departure information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"airport\": {\n      \"$ref\": \"#/components/schemas/ListingAirportContract\"\n    },\n    \"scheduledTime\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    },\n    \"revisedTime\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    },\n    \"predictedTime\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    },\n    \"runwayTime\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    },\n    \"terminal\": {\n      \"type\": \"string\",\n      \"description\": \"Terminal of the flight\",\n      \"nullable\": true\n    },\n\
  \    \"checkInDesk\": {\n      \"type\": \"string\",\n      \"description\": \"Check-in desk(s) for the flight (only for departing flights)\",\n      \"nullable\": true\n    },\n    \"gate\": {\n      \"type\": \"string\",\n      \"description\": \"Gate of (un)boarding for the flight\",\n      \"nullable\": true\n    },\n    \"baggageBelt\": {\n      \"type\": \"string\",\n      \"description\": \"Baggage belt(s) for the flight (only for arriving flights)\",\n      \"nullable\": true\n    },\n    \"runway\": {\n      \"type\": \"string\",\n      \"description\": \"Name of a runway of landing (for arriving flights) or take-off (for departing flights), if known.\",\n      \"nullable\": true\n    },\n    \"quality\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FlightAirportMovementQualityEnum\"\n      },\n      \"description\": \"Array of quality characteristics of the data. Check this to know which information\\r\\nyou can expect within this\
  \ contract (basic, live and/or approximate data).\"\n    }\n  },\n  \"required\": [\n    \"airport\",\n    \"quality\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-airport-movement-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FlightAirportMovementContract
---
