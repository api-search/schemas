---
description: Solar information at the moment
layout: schema
name: SolarStateContract
properties_list:
- description: ''
  name: location
  type: object
- description: ''
  name: sunElevation
  type: object
- description: ''
  name: sunAzimuth
  type: object
- description: Daytime states
  name: dayTime
  type: array
- description: ''
  name: dawnAstronomical
  type: object
- description: ''
  name: dawnNautical
  type: object
- description: ''
  name: dawnCivil
  type: object
- description: ''
  name: sunrise
  type: object
- description: ''
  name: noonTrue
  type: object
- description: ''
  name: sunset
  type: object
- description: ''
  name: duskCivil
  type: object
- description: ''
  name: duskNautical
  type: object
- description: ''
  name: duskAstronomical
  type: object
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-solar-state-contract-schema.json
slug: aerodatabox-solar-state-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-solar-state-contract-schema.json\",\n  \"title\": \"SolarStateContract\",\n  \"description\": \"Solar information at the moment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"location\": {\n      \"$ref\": \"#/components/schemas/GeoCoordinatesContract\"\n    },\n    \"sunElevation\": {\n      \"$ref\": \"#/components/schemas/Angle\"\n    },\n    \"sunAzimuth\": {\n      \"$ref\": \"#/components/schemas/Azimuth\"\n    },\n    \"dayTime\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DayTime\"\n      },\n      \"description\": \"Daytime states\"\n    },\n    \"dawnAstronomical\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    },\n    \"dawnNautical\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    },\n \
  \   \"dawnCivil\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    },\n    \"sunrise\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    },\n    \"noonTrue\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    },\n    \"sunset\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    },\n    \"duskCivil\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    },\n    \"duskNautical\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    },\n    \"duskAstronomical\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    }\n  },\n  \"required\": [\n    \"dayTime\",\n    \"location\",\n    \"sunAzimuth\",\n    \"sunElevation\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-solar-state-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: SolarStateContract
---
