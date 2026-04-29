---
description: A point in time on a weekly schedule
layout: schema
name: Point
properties_list:
- description: Day of the week (0=Sunday, 6=Saturday)
  name: day
  type: integer
- description: Hour in 24-hour format (0-23)
  name: hour
  type: integer
- description: Minute (0-59)
  name: minute
  type: integer
- description: A specific date for current opening hours
  name: date
  type: object
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-point-schema.json
slug: google-maps-places-point
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Point\",\n  \"type\": \"object\",\n  \"description\": \"A point in time on a weekly schedule\",\n  \"properties\": {\n    \"day\": {\n      \"type\": \"integer\",\n      \"description\": \"Day of the week (0=Sunday, 6=Saturday)\"\n    },\n    \"hour\": {\n      \"type\": \"integer\",\n      \"description\": \"Hour in 24-hour format (0-23)\"\n    },\n    \"minute\": {\n      \"type\": \"integer\",\n      \"description\": \"Minute (0-59)\"\n    },\n    \"date\": {\n      \"type\": \"object\",\n      \"description\": \"A specific date for current opening hours\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-point-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: Point
---
