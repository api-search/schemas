---
description: Single airport data
layout: schema
name: AirportContract
properties_list:
- description: ICAO code of the airport
  name: icao
  type: string
- description: IATA code of the airport
  name: iata
  type: string
- description: Code of the airport within the local or national coding system
  name: localCode
  type: string
- description: Shortened name of the airport
  name: shortName
  type: string
- description: Full name of the airport (derived from own airport name and municipality name)
  name: fullName
  type: string
- description: Name of the municipality this airport belongs to
  name: municipalityName
  type: string
- description: ''
  name: location
  type: object
- description: ''
  name: elevation
  type: object
- description: ''
  name: country
  type: object
- description: ''
  name: continent
  type: object
- description: Time zone of the airport in Olson format (e.g. "Europe/Amsterdam")
  name: timeZone
  type: string
- description: ''
  name: urls
  type: object
- description: List of runway information, if requested
  name: runways
  type: array
- description: ''
  name: currentTime
  type: object
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-airport-contract-schema.json
slug: aerodatabox-airport-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-contract-schema.json\",\n  \"title\": \"AirportContract\",\n  \"description\": \"Single airport data\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"icao\": {\n      \"type\": \"string\",\n      \"description\": \"ICAO code of the airport\",\n      \"nullable\": true\n    },\n    \"iata\": {\n      \"type\": \"string\",\n      \"description\": \"IATA code of the airport\",\n      \"nullable\": true\n    },\n    \"localCode\": {\n      \"type\": \"string\",\n      \"description\": \"Code of the airport within the local or national coding system\",\n      \"nullable\": true\n    },\n    \"shortName\": {\n      \"type\": \"string\",\n      \"description\": \"Shortened name of the airport\",\n      \"nullable\": true\n    },\n    \"fullName\": {\n      \"minLength\": 1,\n      \"type\"\
  : \"string\",\n      \"description\": \"Full name of the airport (derived from own airport name and municipality name)\"\n    },\n    \"municipalityName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the municipality this airport belongs to\",\n      \"nullable\": true\n    },\n    \"location\": {\n      \"$ref\": \"#/components/schemas/GeoCoordinatesContract\"\n    },\n    \"elevation\": {\n      \"$ref\": \"#/components/schemas/Distance\"\n    },\n    \"country\": {\n      \"$ref\": \"#/components/schemas/CountryContract\"\n    },\n    \"continent\": {\n      \"$ref\": \"#/components/schemas/ContinentContract\"\n    },\n    \"timeZone\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Time zone of the airport in Olson format (e.g. \\\"Europe/Amsterdam\\\")\"\n    },\n    \"urls\": {\n      \"$ref\": \"#/components/schemas/AirportUrlsContract\"\n    },\n    \"runways\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"\
  $ref\": \"#/components/schemas/RunwayContract\"\n      },\n      \"description\": \"List of runway information, if requested\",\n      \"nullable\": true\n    },\n    \"currentTime\": {\n      \"$ref\": \"#/components/schemas/AirportLocalTimeContract\"\n    }\n  },\n  \"required\": [\n    \"continent\",\n    \"country\",\n    \"elevation\",\n    \"fullName\",\n    \"location\",\n    \"timeZone\",\n    \"urls\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: AirportContract
---
