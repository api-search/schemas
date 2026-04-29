---
description: An encoded polyline representation of a route or step
layout: schema
name: Polyline
properties_list:
- description: An encoded polyline string using the Encoded Polyline Algorithm. Decode to obtain a series of lat/lng coordinates.
  name: points
  type: string
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-directions-polyline-schema.json
slug: google-maps-directions-polyline
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Polyline\",\n  \"type\": \"object\",\n  \"description\": \"An encoded polyline representation of a route or step\",\n  \"properties\": {\n    \"points\": {\n      \"type\": \"string\",\n      \"description\": \"An encoded polyline string using the Encoded Polyline Algorithm. Decode to obtain a series of lat/lng coordinates.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-directions-polyline-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: Polyline
---
