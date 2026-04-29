---
description: Statistical record of route daily statistics
layout: schema
name: DailyRouteStatRecordContract
properties_list:
- description: ''
  name: destination
  type: object
- description: Daily average of flights per destination
  name: averageDailyFlights
  type: number
- description: Airlines operating on the route
  name: operators
  type: array
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-daily-route-stat-record-contract-schema.json
slug: aerodatabox-daily-route-stat-record-contract
source_filename: aerodatabox-daily-route-stat-record-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-daily-route-stat-record-contract-schema.json\",\n  \"title\": \"DailyRouteStatRecordContract\",\n  \"description\": \"Statistical record of route daily statistics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destination\": {\n      \"$ref\": \"#/components/schemas/ListingAirportContract\"\n    },\n    \"averageDailyFlights\": {\n      \"type\": \"number\",\n      \"description\": \"Daily average of flights per destination\",\n      \"format\": \"float\"\n    },\n    \"operators\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FlightAirlineContract\"\n      },\n      \"description\": \"Airlines operating on the route\"\n    }\n  },\n  \"required\": [\n    \"averageDailyFlights\",\n    \"destination\",\n    \"operators\"\n  ],\n  \"additionalProperties\"\
  : false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-daily-route-stat-record-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: DailyRouteStatRecordContract
---
