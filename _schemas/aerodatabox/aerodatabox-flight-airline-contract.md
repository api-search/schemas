---
description: Flight's airline reference conract
layout: schema
name: FlightAirlineContract
properties_list:
- description: Airline name
  name: name
  type: string
- description: IATA code of the airline
  name: iata
  type: string
- description: ICAO code of the airline
  name: icao
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-flight-airline-contract-schema.json
slug: aerodatabox-flight-airline-contract
source_filename: aerodatabox-flight-airline-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-airline-contract-schema.json\",\n  \"title\": \"FlightAirlineContract\",\n  \"description\": \"Flight's airline reference conract\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Airline name\"\n    },\n    \"iata\": {\n      \"type\": \"string\",\n      \"description\": \"IATA code of the airline\",\n      \"nullable\": true\n    },\n    \"icao\": {\n      \"type\": \"string\",\n      \"description\": \"ICAO code of the airline\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-airline-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FlightAirlineContract
---
