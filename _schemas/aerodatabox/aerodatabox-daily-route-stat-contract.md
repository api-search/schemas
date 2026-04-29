---
description: Route daily statistics of the airport
layout: schema
name: DailyRouteStatContract
properties_list:
- description: ''
  name: routes
  type: array
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-daily-route-stat-contract-schema.json
slug: aerodatabox-daily-route-stat-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-daily-route-stat-contract-schema.json\",\n  \"title\": \"DailyRouteStatContract\",\n  \"description\": \"Route daily statistics of the airport\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"routes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DailyRouteStatRecordContract\"\n      }\n    }\n  },\n  \"required\": [\n    \"routes\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-daily-route-stat-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: DailyRouteStatContract
---
