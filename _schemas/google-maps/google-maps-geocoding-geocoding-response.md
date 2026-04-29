---
description: The response from the Geocoding API
layout: schema
name: GeocodingResponse
properties_list:
- description: Status code indicating the outcome of the request.
  name: status
  type: string
- description: Array of geocoded address results
  name: results
  type: array
- description: Human-readable description of the error, present when status is not OK.
  name: error_message
  type: string
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-geocoding-geocoding-response-schema.json
slug: google-maps-geocoding-geocoding-response
source_filename: google-maps-geocoding-geocoding-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GeocodingResponse\",\n  \"type\": \"object\",\n  \"description\": \"The response from the Geocoding API\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status code indicating the outcome of the request.\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Array of geocoded address results\"\n    },\n    \"error_message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the error, present when status is not OK.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-geocoding-geocoding-response-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: GeocodingResponse
---
