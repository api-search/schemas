---
description: Parking options at a place
layout: schema
name: ParkingOptions
properties_list:
- description: ''
  name: freeParkingLot
  type: boolean
- description: ''
  name: paidParkingLot
  type: boolean
- description: ''
  name: freeStreetParking
  type: boolean
- description: ''
  name: paidStreetParking
  type: boolean
- description: ''
  name: valetParking
  type: boolean
- description: ''
  name: freeGarageParking
  type: boolean
- description: ''
  name: paidGarageParking
  type: boolean
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-parking-options-schema.json
slug: google-maps-places-parking-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ParkingOptions\",\n  \"type\": \"object\",\n  \"description\": \"Parking options at a place\",\n  \"properties\": {\n    \"freeParkingLot\": {\n      \"type\": \"boolean\"\n    },\n    \"paidParkingLot\": {\n      \"type\": \"boolean\"\n    },\n    \"freeStreetParking\": {\n      \"type\": \"boolean\"\n    },\n    \"paidStreetParking\": {\n      \"type\": \"boolean\"\n    },\n    \"valetParking\": {\n      \"type\": \"boolean\"\n    },\n    \"freeGarageParking\": {\n      \"type\": \"boolean\"\n    },\n    \"paidGarageParking\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-parking-options-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: ParkingOptions
---
