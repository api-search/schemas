---
description: A coach route between two stations in the BlaBlaCar Bus network
layout: schema
name: Route
properties_list:
- description: Unique route identifier
  name: id
  type: string
- description: Origin station identifier
  name: from_station_id
  type: string
- description: Destination station identifier
  name: to_station_id
  type: string
- description: Typical route duration in minutes
  name: duration_minutes
  type: integer
- description: Route distance in kilometers
  name: distance_km
  type: integer
provider_name: BlaBlaCar Bus API
provider_slug: blablacar-bus-api
schema_file: json-schema/blablacar-bus-api-route-schema.json
slug: blablacar-bus-api-route
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/json-schema/blablacar-bus-api-route-schema.json\",\n  \"title\": \"Route\",\n  \"description\": \"A coach route between two stations in the BlaBlaCar Bus network\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique route identifier\",\n      \"example\": \"route-paris-lyon\"\n    },\n    \"from_station_id\": {\n      \"type\": \"string\",\n      \"description\": \"Origin station identifier\",\n      \"example\": \"FRTLS\"\n    },\n    \"to_station_id\": {\n      \"type\": \"string\",\n      \"description\": \"Destination station identifier\",\n      \"example\": \"FRLYO\"\n    },\n    \"duration_minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Typical route duration in minutes\",\n      \"example\": 180\n    },\n    \"distance_km\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Route distance in kilometers\",\n      \"example\": 465\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"from_station_id\",\n    \"to_station_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/json-schema/blablacar-bus-api-route-schema.json
tags:
- Booking
- Buses
- Coach
- Europe
- Mobility
- Ticketing
- Transportation
- Travel
title: Route
---
