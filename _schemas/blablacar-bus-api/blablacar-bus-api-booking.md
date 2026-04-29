---
description: A confirmed booking for one or more passengers on a BlaBlaCar Bus trip
layout: schema
name: Booking
properties_list:
- description: Unique booking identifier
  name: booking_id
  type: string
- description: Current booking status
  name: status
  type: string
- description: Partner's own reference identifier
  name: partner_reference
  type: string
- description: Total booking price
  name: total_price
  type: object
provider_name: BlaBlaCar Bus API
provider_slug: blablacar-bus-api
schema_file: json-schema/blablacar-bus-api-booking-schema.json
slug: blablacar-bus-api-booking
source_filename: blablacar-bus-api-booking-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/json-schema/blablacar-bus-api-booking-schema.json\",\n  \"title\": \"Booking\",\n  \"description\": \"A confirmed booking for one or more passengers on a BlaBlaCar Bus trip\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"booking_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique booking identifier\",\n      \"example\": \"booking-500123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current booking status\",\n      \"enum\": [\n        \"confirmed\",\n        \"pending\",\n        \"cancelled\"\n      ],\n      \"example\": \"confirmed\"\n    },\n    \"partner_reference\": {\n      \"type\": \"string\",\n      \"description\": \"Partner's own reference identifier\",\n      \"example\": \"booking-ref-abc123\"\n    },\n    \"total_price\": {\n      \"\
  type\": \"object\",\n      \"description\": \"Total booking price\",\n      \"properties\": {\n        \"amount\": {\n          \"type\": \"integer\",\n          \"example\": 1299\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"example\": \"EUR\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"booking_id\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/json-schema/blablacar-bus-api-booking-schema.json
tags:
- Booking
- Buses
- Coach
- Europe
- Mobility
- Ticketing
- Transportation
- Travel
title: Booking
---
