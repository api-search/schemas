---
description: A place prediction
layout: schema
name: PlacePrediction
properties_list:
- description: The resource name of the suggested place in the format places/{placeId}
  name: place
  type: string
- description: The place ID of the suggested place
  name: placeId
  type: string
- description: List of types that apply to this place
  name: types
  type: array
- description: The distance in meters from the origin
  name: distanceMeters
  type: integer
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-place-prediction-schema.json
slug: google-maps-places-place-prediction
source_filename: google-maps-places-place-prediction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlacePrediction\",\n  \"type\": \"object\",\n  \"description\": \"A place prediction\",\n  \"properties\": {\n    \"place\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the suggested place in the format places/{placeId}\"\n    },\n    \"placeId\": {\n      \"type\": \"string\",\n      \"description\": \"The place ID of the suggested place\"\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"List of types that apply to this place\"\n    },\n    \"distanceMeters\": {\n      \"type\": \"integer\",\n      \"description\": \"The distance in meters from the origin\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-place-prediction-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: PlacePrediction
---
