---
description: Azimuth schema from AeroDataBox API
layout: schema
name: Azimuth
properties_list:
- description: Angle in degrees (between `0` and `360`)
  name: deg
  type: number
- description: Angle in radians (`0` and `2 * Pi`)
  name: rad
  type: number
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-azimuth-schema.json
slug: aerodatabox-azimuth
source_filename: aerodatabox-azimuth-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-azimuth-schema.json\",\n  \"title\": \"Azimuth\",\n  \"description\": \"Azimuth schema from AeroDataBox API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deg\": {\n      \"maximum\": 360,\n      \"minimum\": 0,\n      \"type\": \"number\",\n      \"description\": \"Angle in degrees (between `0` and `360`)\",\n      \"format\": \"double\"\n    },\n    \"rad\": {\n      \"maximum\": 6.283185307179586,\n      \"minimum\": 0,\n      \"type\": \"number\",\n      \"description\": \"Angle in radians (`0` and `2 * Pi`)\",\n      \"format\": \"double\"\n    }\n  },\n  \"required\": [\n    \"deg\",\n    \"rad\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-azimuth-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: Azimuth
---
