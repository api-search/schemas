---
description: Single aircraft data
layout: schema
name: AircraftContract
properties_list:
- description: Unique ID of the aircraft record in our database
  name: id
  type: integer
- description: Tail-number of the aircraft
  name: reg
  type: string
- description: Indicator if aircraft is operational under this registration
  name: active
  type: boolean
- description: Serial number
  name: serial
  type: string
- description: ICAO 24 bit Mode-S hexadecimal transponder address
  name: hexIcao
  type: string
- description: Name of the airline operating the aircraft
  name: airlineName
  type: string
- description: IATA-type of the aircraft
  name: iataType
  type: string
- description: Short variant of IATA-code of the aircraft
  name: iataCodeShort
  type: string
- description: ICAO-code of the aircraft
  name: icaoCode
  type: string
- description: Model of the aircraft
  name: model
  type: string
- description: Model code of the aircraft
  name: modelCode
  type: string
- description: Number of passenger seats
  name: numSeats
  type: integer
- description: Date of roll-out (UTC)
  name: rolloutDate
  type: string
- description: First flight date
  name: firstFlightDate
  type: string
- description: Date of delivery to the owner
  name: deliveryDate
  type: string
- description: Date of assigning current registration
  name: registrationDate
  type: string
- description: Type name
  name: typeName
  type: string
- description: Number of engines
  name: numEngines
  type: integer
- description: ''
  name: engineType
  type: object
- description: Marker if aircraft is cargo or not
  name: isFreighter
  type: boolean
- description: Production line
  name: productionLine
  type: string
- description: Age of the aircraft in year
  name: ageYears
  type: number
- description: ''
  name: verified
  type: boolean
- description: ''
  name: image
  type: object
- description: An aircraft may have a history of past registrations with other airlines or operators. This field represents a total number of registration records known in our database.
  name: numRegistrations
  type: integer
- description: A history of all registrations with other airlines or operators (if provided by the endpoint).
  name: registrations
  type: array
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-aircraft-contract-schema.json
slug: aerodatabox-aircraft-contract
source_filename: aerodatabox-aircraft-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-aircraft-contract-schema.json\",\n  \"title\": \"AircraftContract\",\n  \"description\": \"Single aircraft data\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique ID of the aircraft record in our database\",\n      \"format\": \"int64\"\n    },\n    \"reg\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Tail-number of the aircraft\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicator if aircraft is operational under this registration\"\n    },\n    \"serial\": {\n      \"type\": \"string\",\n      \"description\": \"Serial number\",\n      \"nullable\": true\n    },\n    \"hexIcao\": {\n      \"type\": \"string\",\n      \"description\": \"ICAO\
  \ 24 bit Mode-S hexadecimal transponder address\",\n      \"nullable\": true\n    },\n    \"airlineName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the airline operating the aircraft\",\n      \"nullable\": true\n    },\n    \"iataType\": {\n      \"type\": \"string\",\n      \"description\": \"IATA-type of the aircraft\",\n      \"nullable\": true\n    },\n    \"iataCodeShort\": {\n      \"type\": \"string\",\n      \"description\": \"Short variant of IATA-code of the aircraft\",\n      \"nullable\": true\n    },\n    \"icaoCode\": {\n      \"type\": \"string\",\n      \"description\": \"ICAO-code of the aircraft\",\n      \"nullable\": true\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Model of the aircraft\",\n      \"nullable\": true\n    },\n    \"modelCode\": {\n      \"type\": \"string\",\n      \"description\": \"Model code of the aircraft\",\n      \"nullable\": true\n    },\n    \"numSeats\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Number of passenger seats\",\n      \"format\": \"int32\",\n      \"nullable\": true\n    },\n    \"rolloutDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of roll-out (UTC)\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"firstFlightDate\": {\n      \"type\": \"string\",\n      \"description\": \"First flight date\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"deliveryDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of delivery to the owner\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"registrationDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of assigning current registration\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"typeName\": {\n      \"type\": \"string\",\n      \"description\": \"Type name\",\n      \"nullable\": true\n    },\n    \"numEngines\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Number of engines\",\n      \"format\": \"int32\",\n      \"nullable\": true\n    },\n    \"engineType\": {\n      \"$ref\": \"#/components/schemas/EngineType\"\n    },\n    \"isFreighter\": {\n      \"type\": \"boolean\",\n      \"description\": \"Marker if aircraft is cargo or not\"\n    },\n    \"productionLine\": {\n      \"type\": \"string\",\n      \"description\": \"Production line\",\n      \"nullable\": true\n    },\n    \"ageYears\": {\n      \"type\": \"number\",\n      \"description\": \"Age of the aircraft in year\",\n      \"format\": \"float\",\n      \"nullable\": true\n    },\n    \"verified\": {\n      \"type\": \"boolean\"\n    },\n    \"image\": {\n      \"$ref\": \"#/components/schemas/ResourceContract\"\n    },\n    \"numRegistrations\": {\n      \"type\": \"integer\",\n      \"description\": \"An aircraft may have a history of past registrations with other airlines or operators.\\r\\nThis field represents a total number of\
  \ registration records known in our database.\",\n      \"format\": \"int32\"\n    },\n    \"registrations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AircraftRegistrationContract\"\n      },\n      \"description\": \"A history of all registrations with other airlines or operators (if provided by the endpoint).\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"active\",\n    \"id\",\n    \"isFreighter\",\n    \"numRegistrations\",\n    \"reg\",\n    \"verified\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-aircraft-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: AircraftContract
---
