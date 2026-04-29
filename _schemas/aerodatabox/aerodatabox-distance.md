---
description: Distance schema from AeroDataBox API
layout: schema
name: Distance
properties_list:
- description: Distance in meters
  name: meter
  type: number
- description: Distance in kilometers
  name: km
  type: number
- description: Distance in statute miles
  name: mile
  type: number
- description: Distance in nautical miles
  name: nm
  type: number
- description: Distance in feet
  name: feet
  type: number
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-distance-schema.json
slug: aerodatabox-distance
source_filename: aerodatabox-distance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-distance-schema.json\",\n  \"title\": \"Distance\",\n  \"description\": \"Distance schema from AeroDataBox API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"meter\": {\n      \"type\": \"number\",\n      \"description\": \"Distance in meters\",\n      \"format\": \"double\"\n    },\n    \"km\": {\n      \"type\": \"number\",\n      \"description\": \"Distance in kilometers\",\n      \"format\": \"double\"\n    },\n    \"mile\": {\n      \"type\": \"number\",\n      \"description\": \"Distance in statute miles\",\n      \"format\": \"double\"\n    },\n    \"nm\": {\n      \"type\": \"number\",\n      \"description\": \"Distance in nautical miles\",\n      \"format\": \"double\"\n    },\n    \"feet\": {\n      \"type\": \"number\",\n      \"description\": \"Distance in feet\",\n      \"\
  format\": \"double\"\n    }\n  },\n  \"required\": [\n    \"feet\",\n    \"km\",\n    \"meter\",\n    \"mile\",\n    \"nm\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-distance-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: Distance
---
