---
description: The total fare for a transit route
layout: schema
name: Fare
properties_list:
- description: ISO 4217 currency code
  name: currency
  type: string
- description: The total fare amount in the specified currency
  name: value
  type: number
- description: Human-readable fare text
  name: text
  type: string
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-directions-fare-schema.json
slug: google-maps-directions-fare
source_filename: google-maps-directions-fare-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Fare\",\n  \"type\": \"object\",\n  \"description\": \"The total fare for a transit route\",\n  \"properties\": {\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"The total fare amount in the specified currency\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable fare text\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-directions-fare-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: Fare
---
