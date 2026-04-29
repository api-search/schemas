---
description: Contract describing unit (altitude, airspeed, etc.) which can be assigned and / or requested in the context of the flight plan
layout: schema
name: DistanceFlightPlanUnitContract
properties_list:
- description: ''
  name: requested
  type: object
- description: ''
  name: assigned
  type: object
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-distance-flight-plan-unit-contract-schema.json
slug: aerodatabox-distance-flight-plan-unit-contract
source_filename: aerodatabox-distance-flight-plan-unit-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-distance-flight-plan-unit-contract-schema.json\",\n  \"title\": \"DistanceFlightPlanUnitContract\",\n  \"description\": \"Contract describing unit (altitude, airspeed, etc.) which can be assigned and / or requested\\r\\nin the context of the flight plan\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requested\": {\n      \"$ref\": \"#/components/schemas/Distance\"\n    },\n    \"assigned\": {\n      \"$ref\": \"#/components/schemas/Distance\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-distance-flight-plan-unit-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: DistanceFlightPlanUnitContract
---
