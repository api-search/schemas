---
description: Geocoded information for a waypoint
layout: schema
name: GeocodedWaypoint
properties_list:
- description: Status of the geocoding operation
  name: geocoder_status
  type: string
- description: Place ID of the geocoded waypoint
  name: place_id
  type: string
- description: Address type(s) of the geocoded waypoint
  name: types
  type: array
- description: Whether the geocoder did not return an exact match
  name: partial_match
  type: boolean
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-directions-geocoded-waypoint-schema.json
slug: google-maps-directions-geocoded-waypoint
source_filename: google-maps-directions-geocoded-waypoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GeocodedWaypoint\",\n  \"type\": \"object\",\n  \"description\": \"Geocoded information for a waypoint\",\n  \"properties\": {\n    \"geocoder_status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the geocoding operation\"\n    },\n    \"place_id\": {\n      \"type\": \"string\",\n      \"description\": \"Place ID of the geocoded waypoint\"\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"Address type(s) of the geocoded waypoint\"\n    },\n    \"partial_match\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the geocoder did not return an exact match\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-directions-geocoded-waypoint-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: GeocodedWaypoint
---
