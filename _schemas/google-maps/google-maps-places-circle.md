---
description: A circle defined by center point and radius
layout: schema
name: Circle
properties_list:
- description: The radius of the circle in meters
  name: radius
  type: number
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-circle-schema.json
slug: google-maps-places-circle
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Circle\",\n  \"type\": \"object\",\n  \"description\": \"A circle defined by center point and radius\",\n  \"properties\": {\n    \"radius\": {\n      \"type\": \"number\",\n      \"description\": \"The radius of the circle in meters\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-circle-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: Circle
---
