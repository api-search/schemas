---
description: Descriptor date-time represented in both UTC and local timezones
layout: schema
name: DateTimeContract
properties_list:
- description: UTC-time
  name: utc
  type: string
- description: Local time
  name: local
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-date-time-contract-schema.json
slug: aerodatabox-date-time-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-date-time-contract-schema.json\",\n  \"title\": \"DateTimeContract\",\n  \"description\": \"Descriptor date-time represented in both UTC and local timezones\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"utc\": {\n      \"type\": \"string\",\n      \"description\": \"UTC-time\",\n      \"format\": \"date-time\"\n    },\n    \"local\": {\n      \"type\": \"string\",\n      \"description\": \"Local time\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"local\",\n    \"utc\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-date-time-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: DateTimeContract
---
