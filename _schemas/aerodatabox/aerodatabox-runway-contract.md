---
description: Single runway data
layout: schema
name: RunwayContract
properties_list:
- description: 'Name of the runway. E.g.: 27L, 06, 36C, etc.'
  name: name
  type: string
- description: True heading of the runway in degrees
  name: trueHdg
  type: number
- description: ''
  name: length
  type: object
- description: ''
  name: width
  type: object
- description: Marker, if runway is closed
  name: isClosed
  type: boolean
- description: ''
  name: location
  type: object
- description: ''
  name: surface
  type: object
- description: ''
  name: displacedThreshold
  type: object
- description: Does runway has lights
  name: hasLighting
  type: boolean
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-runway-contract-schema.json
slug: aerodatabox-runway-contract
source_filename: aerodatabox-runway-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-runway-contract-schema.json\",\n  \"title\": \"RunwayContract\",\n  \"description\": \"Single runway data\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Name of the runway. E.g.: 27L, 06, 36C, etc.\"\n    },\n    \"trueHdg\": {\n      \"type\": \"number\",\n      \"description\": \"True heading of the runway in degrees\",\n      \"format\": \"double\"\n    },\n    \"length\": {\n      \"$ref\": \"#/components/schemas/Distance\"\n    },\n    \"width\": {\n      \"$ref\": \"#/components/schemas/Distance\"\n    },\n    \"isClosed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Marker, if runway is closed\"\n    },\n    \"location\": {\n      \"$ref\": \"#/components/schemas/GeoCoordinatesContract\"\
  \n    },\n    \"surface\": {\n      \"$ref\": \"#/components/schemas/SurfaceType\"\n    },\n    \"displacedThreshold\": {\n      \"$ref\": \"#/components/schemas/Distance\"\n    },\n    \"hasLighting\": {\n      \"type\": \"boolean\",\n      \"description\": \"Does runway has lights\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"isClosed\",\n    \"name\",\n    \"surface\",\n    \"trueHdg\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-runway-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: RunwayContract
---
