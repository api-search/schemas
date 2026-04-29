---
description: Geographical coordinates data
layout: schema
name: GeoCoordinatesContract
properties_list:
- description: Latitude, in degrees
  name: lat
  type: number
- description: Longitude, in degrees
  name: lon
  type: number
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-geo-coordinates-contract-schema.json
slug: aerodatabox-geo-coordinates-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-geo-coordinates-contract-schema.json\",\n  \"title\": \"GeoCoordinatesContract\",\n  \"description\": \"Geographical coordinates data\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lat\": {\n      \"maximum\": 90,\n      \"minimum\": -90,\n      \"type\": \"number\",\n      \"description\": \"Latitude, in degrees\",\n      \"format\": \"float\"\n    },\n    \"lon\": {\n      \"maximum\": 180,\n      \"minimum\": -180,\n      \"type\": \"number\",\n      \"description\": \"Longitude, in degrees\",\n      \"format\": \"float\"\n    }\n  },\n  \"required\": [\n    \"lat\",\n    \"lon\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-geo-coordinates-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: GeoCoordinatesContract
---
