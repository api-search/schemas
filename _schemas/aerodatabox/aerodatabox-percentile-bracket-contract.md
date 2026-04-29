---
description: Percentile bracket contract describing the flight delay for a specific percentile of the distribution
layout: schema
name: PercentileBracketContract
properties_list:
- description: Percentile of the distribution
  name: percentile
  type: integer
- description: 'Delay of the flight for the specific percentile (format: [-]hh:mm:ss).'
  name: delay
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-percentile-bracket-contract-schema.json
slug: aerodatabox-percentile-bracket-contract
source_filename: aerodatabox-percentile-bracket-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-percentile-bracket-contract-schema.json\",\n  \"title\": \"PercentileBracketContract\",\n  \"description\": \"Percentile bracket contract describing the flight delay for a specific percentile of the distribution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"percentile\": {\n      \"maximum\": 95,\n      \"minimum\": 5,\n      \"type\": \"integer\",\n      \"description\": \"Percentile of the distribution\",\n      \"format\": \"int32\"\n    },\n    \"delay\": {\n      \"type\": \"string\",\n      \"description\": \"Delay of the flight for the specific percentile (format: [-]hh:mm:ss).\",\n      \"format\": \"date-span\"\n    }\n  },\n  \"required\": [\n    \"delay\",\n    \"percentile\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-percentile-bracket-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: PercentileBracketContract
---
