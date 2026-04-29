---
description: A specific coach departure on a route with pricing and availability
layout: schema
name: Trip
properties_list:
- description: Unique trip identifier
  name: id
  type: string
- description: Associated route identifier
  name: route_id
  type: string
- description: Departure date and time
  name: departure_datetime
  type: string
- description: Arrival date and time
  name: arrival_datetime
  type: string
- description: Number of seats currently available
  name: available_seats
  type: integer
- description: Price with amount and currency
  name: price
  type: object
provider_name: BlaBlaCar Bus API
provider_slug: blablacar-bus-api
schema_file: json-schema/blablacar-bus-api-trip-schema.json
slug: blablacar-bus-api-trip
source_filename: blablacar-bus-api-trip-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/json-schema/blablacar-bus-api-trip-schema.json\",\n  \"title\": \"Trip\",\n  \"description\": \"A specific coach departure on a route with pricing and availability\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique trip identifier\",\n      \"example\": \"trip-500123\"\n    },\n    \"route_id\": {\n      \"type\": \"string\",\n      \"description\": \"Associated route identifier\",\n      \"example\": \"route-paris-lyon\"\n    },\n    \"departure_datetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Departure date and time\",\n      \"example\": \"2025-06-15T07:00:00Z\"\n    },\n    \"arrival_datetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Arrival date and time\",\n      \"example\": \"2025-06-15T10:00:00Z\"\n    },\n    \"available_seats\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of seats currently available\",\n      \"example\": 24\n    },\n    \"price\": {\n      \"type\": \"object\",\n      \"description\": \"Price with amount and currency\",\n      \"properties\": {\n        \"amount\": {\n          \"type\": \"integer\",\n          \"example\": 1299\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"example\": \"EUR\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"route_id\",\n    \"departure_datetime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/json-schema/blablacar-bus-api-trip-schema.json
tags:
- Booking
- Buses
- Coach
- Europe
- Mobility
- Ticketing
- Transportation
- Travel
title: Trip
---
