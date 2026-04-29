---
description: A text and numeric value pair used for distance, duration, and fare amounts
layout: schema
name: TextValuePair
properties_list:
- description: Human-readable text representation
  name: text
  type: string
- description: Numeric value. For distance, expressed in meters. For duration, expressed in seconds. For fare, expressed in the currency indicated.
  name: value
  type: number
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-directions-text-value-pair-schema.json
slug: google-maps-directions-text-value-pair
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TextValuePair\",\n  \"type\": \"object\",\n  \"description\": \"A text and numeric value pair used for distance, duration, and fare amounts\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable text representation\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Numeric value. For distance, expressed in meters. For duration, expressed in seconds. For fare, expressed in the currency indicated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-directions-text-value-pair-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: TextValuePair
---
