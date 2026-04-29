---
description: Contract containing information on distance and approximate flight time between specified airports
layout: schema
name: AirportDistanceTimeContract
properties_list:
- description: ''
  name: from
  type: object
- description: ''
  name: to
  type: object
- description: ''
  name: greatCircleDistance
  type: object
- description: Approximate flight time based on re-calculation of great circle distance against statistical duration average of multiple flights covered similar distance before.
  name: approxFlightTime
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-airport-distance-time-contract-schema.json
slug: aerodatabox-airport-distance-time-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-distance-time-contract-schema.json\",\n  \"title\": \"AirportDistanceTimeContract\",\n  \"description\": \"Contract containing information on distance and approximate flight time\\r\\nbetween specified airports\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"from\": {\n      \"$ref\": \"#/components/schemas/ListingAirportContract\"\n    },\n    \"to\": {\n      \"$ref\": \"#/components/schemas/ListingAirportContract\"\n    },\n    \"greatCircleDistance\": {\n      \"$ref\": \"#/components/schemas/Distance\"\n    },\n    \"approxFlightTime\": {\n      \"type\": \"string\",\n      \"description\": \"Approximate flight time based on re-calculation of great circle distance\\r\\nagainst statistical duration average of multiple flights covered similar\\r\\ndistance before.\",\n      \"\
  format\": \"date-span\"\n    }\n  },\n  \"required\": [\n    \"approxFlightTime\",\n    \"from\",\n    \"greatCircleDistance\",\n    \"to\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-distance-time-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: AirportDistanceTimeContract
---
