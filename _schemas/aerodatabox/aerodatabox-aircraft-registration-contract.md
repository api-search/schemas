---
description: Aircraft registration data
layout: schema
name: AircraftRegistrationContract
properties_list:
- description: Tail-number of the aircraft
  name: reg
  type: string
- description: Indicator if aircraft is operational under this registration
  name: active
  type: boolean
- description: ICAO 24 bit Mode-S hexadecimal transponder address
  name: hexIcao
  type: string
- description: Name of the airline operating the aircraft
  name: airlineName
  type: string
- description: Date of assigning current registration
  name: registrationDate
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-aircraft-registration-contract-schema.json
slug: aerodatabox-aircraft-registration-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-aircraft-registration-contract-schema.json\",\n  \"title\": \"AircraftRegistrationContract\",\n  \"description\": \"Aircraft registration data\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reg\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Tail-number of the aircraft\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicator if aircraft is operational under this registration\"\n    },\n    \"hexIcao\": {\n      \"type\": \"string\",\n      \"description\": \"ICAO 24 bit Mode-S hexadecimal transponder address\",\n      \"nullable\": true\n    },\n    \"airlineName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the airline operating the aircraft\",\n      \"nullable\": true\n    },\n    \"registrationDate\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Date of assigning current registration\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"active\",\n    \"reg\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-aircraft-registration-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: AircraftRegistrationContract
---
