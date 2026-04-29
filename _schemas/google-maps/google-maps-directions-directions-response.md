---
description: The response from the Directions API
layout: schema
name: DirectionsResponse
properties_list:
- description: Status code of the directions request
  name: status
  type: string
- description: Array of routes from the origin to the destination. Each route contains legs, overview polylines, warnings, and waypoint order.
  name: routes
  type: array
- description: Contains geocoding information for the origin, destination, and each waypoint.
  name: geocoded_waypoints
  type: array
- description: Human-readable error message when status is not OK
  name: error_message
  type: string
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-directions-directions-response-schema.json
slug: google-maps-directions-directions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DirectionsResponse\",\n  \"type\": \"object\",\n  \"description\": \"The response from the Directions API\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status code of the directions request\"\n    },\n    \"routes\": {\n      \"type\": \"array\",\n      \"description\": \"Array of routes from the origin to the destination. Each route contains legs, overview polylines, warnings, and waypoint order.\"\n    },\n    \"geocoded_waypoints\": {\n      \"type\": \"array\",\n      \"description\": \"Contains geocoding information for the origin, destination, and each waypoint.\"\n    },\n    \"error_message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message when status is not OK\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-directions-directions-response-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: DirectionsResponse
---
