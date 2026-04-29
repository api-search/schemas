---
description: Speed schema from AeroDataBox API
layout: schema
name: Speed
properties_list:
- description: Speed in knots
  name: kt
  type: number
- description: Speed in km per hour
  name: kmPerHour
  type: number
- description: Speed in miles per hour
  name: miPerHour
  type: number
- description: Speed in meters per second
  name: meterPerSecond
  type: number
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-speed-schema.json
slug: aerodatabox-speed
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-speed-schema.json\",\n  \"title\": \"Speed\",\n  \"description\": \"Speed schema from AeroDataBox API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kt\": {\n      \"type\": \"number\",\n      \"description\": \"Speed in knots\",\n      \"format\": \"double\"\n    },\n    \"kmPerHour\": {\n      \"type\": \"number\",\n      \"description\": \"Speed in km per hour\",\n      \"format\": \"double\"\n    },\n    \"miPerHour\": {\n      \"type\": \"number\",\n      \"description\": \"Speed in miles per hour\",\n      \"format\": \"double\"\n    },\n    \"meterPerSecond\": {\n      \"type\": \"number\",\n      \"description\": \"Speed in meters per second\",\n      \"format\": \"double\"\n    }\n  },\n  \"required\": [\n    \"kmPerHour\",\n    \"kt\",\n    \"meterPerSecond\",\n    \"miPerHour\"\
  \n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-speed-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: Speed
---
