---
description: Flight record found in the search result.
layout: schema
name: FlightSearchItemContract
properties_list:
- description: Found flight number.
  name: number
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-flight-search-item-contract-schema.json
slug: aerodatabox-flight-search-item-contract
source_filename: aerodatabox-flight-search-item-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-search-item-contract-schema.json\",\n  \"title\": \"FlightSearchItemContract\",\n  \"description\": \"Flight record found in the search result.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"number\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Found flight number.\"\n    }\n  },\n  \"required\": [\n    \"number\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-search-item-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FlightSearchItemContract
---
