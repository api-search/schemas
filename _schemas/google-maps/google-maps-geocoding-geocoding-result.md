---
description: A single geocoding result
layout: schema
name: GeocodingResult
properties_list:
- description: Array of address component objects
  name: address_components
  type: array
- description: The human-readable address of this location, composed from the individual address components.
  name: formatted_address
  type: string
- description: A unique identifier for this place that can be used with other Google APIs.
  name: place_id
  type: string
- description: Array of feature types describing the address component. See the list of supported types.
  name: types
  type: array
- description: Indicates that the geocoder did not return an exact match for the original request, though it was able to match part of the requested address.
  name: partial_match
  type: boolean
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-geocoding-geocoding-result-schema.json
slug: google-maps-geocoding-geocoding-result
source_filename: google-maps-geocoding-geocoding-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GeocodingResult\",\n  \"type\": \"object\",\n  \"description\": \"A single geocoding result\",\n  \"properties\": {\n    \"address_components\": {\n      \"type\": \"array\",\n      \"description\": \"Array of address component objects\"\n    },\n    \"formatted_address\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable address of this location, composed from the individual address components.\"\n    },\n    \"place_id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for this place that can be used with other Google APIs.\"\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"Array of feature types describing the address component. See the list of supported types.\"\n    },\n    \"partial_match\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates that the geocoder did not return an exact match\
  \ for the original request, though it was able to match part of the requested address.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-geocoding-geocoding-result-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: GeocodingResult
---
