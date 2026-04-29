---
description: Geometry information about the geocoding result
layout: schema
name: Geometry
properties_list:
- description: The type of location returned. ROOFTOP indicates a precise geocode, RANGE_INTERPOLATED indicates an approximation between two precise points, GEOMETRIC_CENTER indicates a geometric center, and APPROXI
  name: location_type
  type: string
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-geocoding-geometry-schema.json
slug: google-maps-geocoding-geometry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Geometry\",\n  \"type\": \"object\",\n  \"description\": \"Geometry information about the geocoding result\",\n  \"properties\": {\n    \"location_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of location returned. ROOFTOP indicates a precise geocode, RANGE_INTERPOLATED indicates an approximation between two precise points, GEOMETRIC_CENTER indicates a geometric center, and APPROXIMATE indicates an approximation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-geocoding-geometry-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: Geometry
---
