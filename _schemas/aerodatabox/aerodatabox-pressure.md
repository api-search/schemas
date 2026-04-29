---
description: Pressure schema from AeroDataBox API
layout: schema
name: Pressure
properties_list:
- description: Pressure in hectopascals
  name: hPa
  type: number
- description: Pressure in inches mercury
  name: inHg
  type: number
- description: Pressure in millimeters mercury
  name: mmHg
  type: number
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-pressure-schema.json
slug: aerodatabox-pressure
source_filename: aerodatabox-pressure-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-pressure-schema.json\",\n  \"title\": \"Pressure\",\n  \"description\": \"Pressure schema from AeroDataBox API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hPa\": {\n      \"type\": \"number\",\n      \"description\": \"Pressure in hectopascals\",\n      \"format\": \"double\"\n    },\n    \"inHg\": {\n      \"type\": \"number\",\n      \"description\": \"Pressure in inches mercury\",\n      \"format\": \"double\"\n    },\n    \"mmHg\": {\n      \"type\": \"number\",\n      \"description\": \"Pressure in millimeters mercury\",\n      \"format\": \"double\"\n    }\n  },\n  \"required\": [\n    \"hPa\",\n    \"inHg\",\n    \"mmHg\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-pressure-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: Pressure
---
