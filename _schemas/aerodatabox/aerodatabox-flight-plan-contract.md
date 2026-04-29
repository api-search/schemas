---
description: Flight plan contract
layout: schema
name: FlightPlanContract
properties_list:
- description: ''
  name: flightRules
  type: object
- description: ''
  name: flightType
  type: object
- description: No. of revision of the flight plan
  name: revisionNo
  type: integer
- description: ''
  name: status
  type: object
- description: Route information for the flight as filed in the flight plan
  name: route
  type: string
- description: ''
  name: altitude
  type: object
- description: ''
  name: airspeed
  type: object
- description: Time (UTC) of the latest known update to the flight plan
  name: lastUpdatedUtc
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-flight-plan-contract-schema.json
slug: aerodatabox-flight-plan-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-plan-contract-schema.json\",\n  \"title\": \"FlightPlanContract\",\n  \"description\": \"Flight plan contract\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flightRules\": {\n      \"$ref\": \"#/components/schemas/FlightRules\"\n    },\n    \"flightType\": {\n      \"$ref\": \"#/components/schemas/FlightType\"\n    },\n    \"revisionNo\": {\n      \"type\": \"integer\",\n      \"description\": \"No. of revision of the flight plan\",\n      \"format\": \"int32\",\n      \"nullable\": true\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/FlightPlanStatus\"\n    },\n    \"route\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Route information for the flight as filed in the flight plan\"\n    },\n    \"altitude\": {\n      \"$ref\"\
  : \"#/components/schemas/DistanceFlightPlanUnitContract\"\n    },\n    \"airspeed\": {\n      \"$ref\": \"#/components/schemas/SpeedFlightPlanUnitContract\"\n    },\n    \"lastUpdatedUtc\": {\n      \"type\": \"string\",\n      \"description\": \"Time (UTC) of the latest known update to the flight plan\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"lastUpdatedUtc\",\n    \"route\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-plan-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FlightPlanContract
---
