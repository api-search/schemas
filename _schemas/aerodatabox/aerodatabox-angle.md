---
description: Angle schema from AeroDataBox API
layout: schema
name: Angle
properties_list:
- description: Angle in degrees (between `-180` and `180`)
  name: deg
  type: number
- description: Angle in radians (between `-Pi` and `Pi`)
  name: rad
  type: number
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-angle-schema.json
slug: aerodatabox-angle
source_filename: aerodatabox-angle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-angle-schema.json\",\n  \"title\": \"Angle\",\n  \"description\": \"Angle schema from AeroDataBox API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deg\": {\n      \"maximum\": 180,\n      \"minimum\": -180,\n      \"type\": \"number\",\n      \"description\": \"Angle in degrees (between `-180` and `180`)\",\n      \"format\": \"double\"\n    },\n    \"rad\": {\n      \"maximum\": 3.141592653589793,\n      \"minimum\": -3.141592653589793,\n      \"type\": \"number\",\n      \"description\": \"Angle in radians (between `-Pi` and `Pi`)\",\n      \"format\": \"double\"\n    }\n  },\n  \"required\": [\n    \"deg\",\n    \"rad\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-angle-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: Angle
---
