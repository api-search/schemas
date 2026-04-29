---
description: Delay statistics of a flight leg
layout: schema
name: FlightLegDelayContract
properties_list:
- description: Flight number
  name: number
  type: string
- description: Delay statistics of flight on departure at origins
  name: origins
  type: array
- description: Delay statistics of flight on arrival at destinations
  name: destinations
  type: array
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-flight-leg-delay-contract-schema.json
slug: aerodatabox-flight-leg-delay-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-leg-delay-contract-schema.json\",\n  \"title\": \"FlightLegDelayContract\",\n  \"description\": \"Delay statistics of a flight leg\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"number\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Flight number\"\n    },\n    \"origins\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FlightDelayContract\"\n      },\n      \"description\": \"Delay statistics of flight on departure at origins\",\n      \"nullable\": true\n    },\n    \"destinations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FlightDelayContract\"\n      },\n      \"description\": \"Delay statistics of flight on arrival at destinations\",\n      \"\
  nullable\": true\n    }\n  },\n  \"required\": [\n    \"number\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-leg-delay-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FlightLegDelayContract
---
