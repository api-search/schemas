---
description: Flight's aircraft reference contract
layout: schema
name: FlightAircraftContract
properties_list:
- description: Tail-number of the aircraft
  name: reg
  type: string
- description: ICAO 24 bit Mode-S hexadecimal transponder address
  name: modeS
  type: string
- description: Aircraft name and model
  name: model
  type: string
- description: ''
  name: image
  type: object
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-flight-aircraft-contract-schema.json
slug: aerodatabox-flight-aircraft-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-aircraft-contract-schema.json\",\n  \"title\": \"FlightAircraftContract\",\n  \"description\": \"Flight's aircraft reference contract\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reg\": {\n      \"type\": \"string\",\n      \"description\": \"Tail-number of the aircraft\",\n      \"nullable\": true\n    },\n    \"modeS\": {\n      \"type\": \"string\",\n      \"description\": \"ICAO 24 bit Mode-S hexadecimal transponder address\",\n      \"nullable\": true\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Aircraft name and model\",\n      \"nullable\": true\n    },\n    \"image\": {\n      \"$ref\": \"#/components/schemas/ResourceContract\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-aircraft-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FlightAircraftContract
---
