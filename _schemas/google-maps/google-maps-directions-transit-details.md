---
description: Transit-specific information for transit steps
layout: schema
name: TransitDetails
properties_list:
- description: The direction in which to travel on this transit line
  name: headsign
  type: string
- description: The expected number of seconds between departures from the same stop at the current time
  name: headway
  type: integer
- description: The number of stops from departure to arrival
  name: num_stops
  type: integer
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-directions-transit-details-schema.json
slug: google-maps-directions-transit-details
source_filename: google-maps-directions-transit-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransitDetails\",\n  \"type\": \"object\",\n  \"description\": \"Transit-specific information for transit steps\",\n  \"properties\": {\n    \"headsign\": {\n      \"type\": \"string\",\n      \"description\": \"The direction in which to travel on this transit line\"\n    },\n    \"headway\": {\n      \"type\": \"integer\",\n      \"description\": \"The expected number of seconds between departures from the same stop at the current time\"\n    },\n    \"num_stops\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of stops from departure to arrival\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-directions-transit-details-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: TransitDetails
---
