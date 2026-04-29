---
description: Flight notification contract
layout: schema
name: FlightNotificationContract
properties_list:
- description: Modified/created flight notification
  name: flights
  type: array
- description: ''
  name: subscription
  type: object
- description: ''
  name: balance
  type: object
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-flight-notification-contract-schema.json
slug: aerodatabox-flight-notification-contract
source_filename: aerodatabox-flight-notification-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-notification-contract-schema.json\",\n  \"title\": \"FlightNotificationContract\",\n  \"description\": \"Flight notification contract\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flights\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FlightNotificationItemContract\"\n      },\n      \"description\": \"Modified/created flight notification\"\n    },\n    \"subscription\": {\n      \"$ref\": \"#/components/schemas/SubscriptionContract\"\n    },\n    \"balance\": {\n      \"$ref\": \"#/components/schemas/SubscriptionBalanceContract\"\n    }\n  },\n  \"required\": [\n    \"flights\",\n    \"subscription\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-notification-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FlightNotificationContract
---
