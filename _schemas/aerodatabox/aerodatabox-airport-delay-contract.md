---
description: AirportDelayContract schema from AeroDataBox API
layout: schema
name: AirportDelayContract
properties_list:
- description: Airport ICAO code
  name: airportIcao
  type: string
- description: ''
  name: from
  type: object
- description: ''
  name: to
  type: object
- description: ''
  name: departuresDelayInformation
  type: object
- description: ''
  name: arrivalsDelayInformation
  type: object
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-airport-delay-contract-schema.json
slug: aerodatabox-airport-delay-contract
source_filename: aerodatabox-airport-delay-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-delay-contract-schema.json\",\n  \"title\": \"AirportDelayContract\",\n  \"description\": \"AirportDelayContract schema from AeroDataBox API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"airportIcao\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Airport ICAO code\"\n    },\n    \"from\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    },\n    \"to\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    },\n    \"departuresDelayInformation\": {\n      \"$ref\": \"#/components/schemas/FlightBatchDelayContract\"\n    },\n    \"arrivalsDelayInformation\": {\n      \"$ref\": \"#/components/schemas/FlightBatchDelayContract\"\n    }\n  },\n  \"required\": [\n    \"airportIcao\",\n    \"arrivalsDelayInformation\",\n\
  \    \"departuresDelayInformation\",\n    \"from\",\n    \"to\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-delay-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: AirportDelayContract
---
