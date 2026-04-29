---
description: A plus code (Open Location Code)
layout: schema
name: PlusCode
properties_list:
- description: The full plus code (global code)
  name: globalCode
  type: string
- description: The compound plus code with locality reference
  name: compoundCode
  type: string
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-plus-code-schema.json
slug: google-maps-places-plus-code
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlusCode\",\n  \"type\": \"object\",\n  \"description\": \"A plus code (Open Location Code)\",\n  \"properties\": {\n    \"globalCode\": {\n      \"type\": \"string\",\n      \"description\": \"The full plus code (global code)\"\n    },\n    \"compoundCode\": {\n      \"type\": \"string\",\n      \"description\": \"The compound plus code with locality reference\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-plus-code-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: PlusCode
---
