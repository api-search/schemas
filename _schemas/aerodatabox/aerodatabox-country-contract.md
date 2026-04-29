---
description: Country data
layout: schema
name: CountryContract
properties_list:
- description: Code
  name: code
  type: string
- description: Name
  name: name
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-country-contract-schema.json
slug: aerodatabox-country-contract
source_filename: aerodatabox-country-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-country-contract-schema.json\",\n  \"title\": \"CountryContract\",\n  \"description\": \"Country data\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Code\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"code\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-country-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: CountryContract
---
