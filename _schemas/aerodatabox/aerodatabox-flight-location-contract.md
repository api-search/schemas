---
description: 'Positional information about flight: location, altitude, speed and track'
layout: schema
name: FlightLocationContract
properties_list:
- description: ''
  name: pressureAltitude
  type: object
- description: ''
  name: altitude
  type: object
- description: ''
  name: pressure
  type: object
- description: ''
  name: groundSpeed
  type: object
- description: ''
  name: trueTrack
  type: object
- description: Vertical speed, in feet per minute Not set if unknown or zero.
  name: vsiFpm
  type: integer
- description: Time (UTC) of when this positional data was reported
  name: reportedAtUtc
  type: string
- description: Latitude, in degrees
  name: lat
  type: number
- description: Longitude, in degrees
  name: lon
  type: number
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-flight-location-contract-schema.json
slug: aerodatabox-flight-location-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-location-contract-schema.json\",\n  \"title\": \"FlightLocationContract\",\n  \"description\": \"Positional information about flight: location, altitude, speed and track\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pressureAltitude\": {\n      \"$ref\": \"#/components/schemas/Distance\"\n    },\n    \"altitude\": {\n      \"$ref\": \"#/components/schemas/Distance\"\n    },\n    \"pressure\": {\n      \"$ref\": \"#/components/schemas/Pressure\"\n    },\n    \"groundSpeed\": {\n      \"$ref\": \"#/components/schemas/Speed\"\n    },\n    \"trueTrack\": {\n      \"$ref\": \"#/components/schemas/Azimuth\"\n    },\n    \"vsiFpm\": {\n      \"type\": \"integer\",\n      \"description\": \"Vertical speed, in feet per minute\\r\\nNot set if unknown or zero.\",\n      \"format\": \"int32\"\
  ,\n      \"nullable\": true\n    },\n    \"reportedAtUtc\": {\n      \"type\": \"string\",\n      \"description\": \"Time (UTC) of when this positional data was reported\",\n      \"format\": \"date-time\"\n    },\n    \"lat\": {\n      \"maximum\": 90,\n      \"minimum\": -90,\n      \"type\": \"number\",\n      \"description\": \"Latitude, in degrees\",\n      \"format\": \"float\"\n    },\n    \"lon\": {\n      \"maximum\": 180,\n      \"minimum\": -180,\n      \"type\": \"number\",\n      \"description\": \"Longitude, in degrees\",\n      \"format\": \"float\"\n    }\n  },\n  \"required\": [\n    \"altitude\",\n    \"groundSpeed\",\n    \"lat\",\n    \"lon\",\n    \"pressure\",\n    \"pressureAltitude\",\n    \"reportedAtUtc\",\n    \"trueTrack\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-location-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FlightLocationContract
---
