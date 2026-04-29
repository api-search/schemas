---
description: Information about the local time at an airport
layout: schema
name: AirportLocalTimeContract
properties_list:
- description: ''
  name: time
  type: object
- description: Timezone ID of the airport (Olson format)
  name: timeZoneId
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-airport-local-time-contract-schema.json
slug: aerodatabox-airport-local-time-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-local-time-contract-schema.json\",\n  \"title\": \"AirportLocalTimeContract\",\n  \"description\": \"Information about the local time at an airport\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"time\": {\n      \"$ref\": \"#/components/schemas/DateTimeContract\"\n    },\n    \"timeZoneId\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Timezone ID of the airport (Olson format)\"\n    }\n  },\n  \"required\": [\n    \"time\",\n    \"timeZoneId\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-local-time-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: AirportLocalTimeContract
---
