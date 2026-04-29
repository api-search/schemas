---
description: A time value with text representation and time zone
layout: schema
name: TimeZoneTextValue
properties_list:
- description: Human-readable time string
  name: text
  type: string
- description: Time expressed in seconds since epoch
  name: value
  type: integer
- description: The time zone of this time value
  name: time_zone
  type: string
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-directions-time-zone-text-value-schema.json
slug: google-maps-directions-time-zone-text-value
source_filename: google-maps-directions-time-zone-text-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TimeZoneTextValue\",\n  \"type\": \"object\",\n  \"description\": \"A time value with text representation and time zone\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable time string\"\n    },\n    \"value\": {\n      \"type\": \"integer\",\n      \"description\": \"Time expressed in seconds since epoch\"\n    },\n    \"time_zone\": {\n      \"type\": \"string\",\n      \"description\": \"The time zone of this time value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-directions-time-zone-text-value-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: TimeZoneTextValue
---
