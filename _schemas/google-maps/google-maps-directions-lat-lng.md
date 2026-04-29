---
description: A latitude/longitude coordinate pair
layout: schema
name: LatLng
properties_list:
- description: Latitude in decimal degrees
  name: lat
  type: number
- description: Longitude in decimal degrees
  name: lng
  type: number
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-directions-lat-lng-schema.json
slug: google-maps-directions-lat-lng
source_filename: google-maps-directions-lat-lng-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LatLng\",\n  \"type\": \"object\",\n  \"description\": \"A latitude/longitude coordinate pair\",\n  \"properties\": {\n    \"lat\": {\n      \"type\": \"number\",\n      \"description\": \"Latitude in decimal degrees\"\n    },\n    \"lng\": {\n      \"type\": \"number\",\n      \"description\": \"Longitude in decimal degrees\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-directions-lat-lng-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: LatLng
---
