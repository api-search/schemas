---
description: Flight data contract represented in airport schedule
layout: schema
name: AirportFlightContract
properties_list:
- description: ''
  name: movement
  type: object
- description: ''
  name: departure
  type: object
- description: ''
  name: arrival
  type: object
- description: Flight Number
  name: number
  type: string
- description: ATC call-sign of the flight
  name: callSign
  type: string
- description: ''
  name: status
  type: object
- description: ''
  name: codeshareStatus
  type: object
- description: Is cargo flight
  name: isCargo
  type: boolean
- description: ''
  name: aircraft
  type: object
- description: ''
  name: airline
  type: object
- description: ''
  name: location
  type: object
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-airport-flight-contract-schema.json
slug: aerodatabox-airport-flight-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-flight-contract-schema.json\",\n  \"title\": \"AirportFlightContract\",\n  \"description\": \"Flight data contract represented in airport schedule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"movement\": {\n      \"$ref\": \"#/components/schemas/FlightAirportMovementContract\"\n    },\n    \"departure\": {\n      \"$ref\": \"#/components/schemas/FlightAirportMovementContract\"\n    },\n    \"arrival\": {\n      \"$ref\": \"#/components/schemas/FlightAirportMovementContract\"\n    },\n    \"number\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Flight Number\"\n    },\n    \"callSign\": {\n      \"type\": \"string\",\n      \"description\": \"ATC call-sign of the flight\",\n      \"nullable\": true\n    },\n    \"status\": {\n      \"$ref\"\
  : \"#/components/schemas/FlightStatus\"\n    },\n    \"codeshareStatus\": {\n      \"$ref\": \"#/components/schemas/CodeshareStatus\"\n    },\n    \"isCargo\": {\n      \"type\": \"boolean\",\n      \"description\": \"Is cargo flight\"\n    },\n    \"aircraft\": {\n      \"$ref\": \"#/components/schemas/FlightAircraftContract\"\n    },\n    \"airline\": {\n      \"$ref\": \"#/components/schemas/FlightAirlineContract\"\n    },\n    \"location\": {\n      \"$ref\": \"#/components/schemas/FlightLocationContract\"\n    }\n  },\n  \"required\": [\n    \"codeshareStatus\",\n    \"isCargo\",\n    \"number\",\n    \"status\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-flight-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: AirportFlightContract
---
