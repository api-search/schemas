---
description: A leg of a route, representing the journey between two waypoints or the origin/destination.
layout: schema
name: Leg
properties_list:
- description: Array of steps representing each instruction along the leg
  name: steps
  type: array
- description: The human-readable address of the leg's starting point
  name: start_address
  type: string
- description: The human-readable address of the leg's ending point
  name: end_address
  type: string
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-directions-leg-schema.json
slug: google-maps-directions-leg
source_filename: google-maps-directions-leg-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Leg\",\n  \"type\": \"object\",\n  \"description\": \"A leg of a route, representing the journey between two waypoints or the origin/destination.\",\n  \"properties\": {\n    \"steps\": {\n      \"type\": \"array\",\n      \"description\": \"Array of steps representing each instruction along the leg\"\n    },\n    \"start_address\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable address of the leg's starting point\"\n    },\n    \"end_address\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable address of the leg's ending point\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-directions-leg-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: Leg
---
