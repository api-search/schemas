---
description: Request body for nearby search
layout: schema
name: SearchNearbyRequest
properties_list:
- description: Place types to include in results
  name: includedTypes
  type: array
- description: Place types to exclude from results
  name: excludedTypes
  type: array
- description: Primary place types to include
  name: includedPrimaryTypes
  type: array
- description: Primary place types to exclude
  name: excludedPrimaryTypes
  type: array
- description: The language code for results
  name: languageCode
  type: string
- description: The region code for biasing results
  name: regionCode
  type: string
- description: How results should be ranked
  name: rankPreference
  type: string
- description: Maximum number of results (1-20)
  name: maxResultCount
  type: integer
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-search-nearby-request-schema.json
slug: google-maps-places-search-nearby-request
source_filename: google-maps-places-search-nearby-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchNearbyRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for nearby search\",\n  \"properties\": {\n    \"includedTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Place types to include in results\"\n    },\n    \"excludedTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Place types to exclude from results\"\n    },\n    \"includedPrimaryTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Primary place types to include\"\n    },\n    \"excludedPrimaryTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Primary place types to exclude\"\n    },\n    \"languageCode\": {\n      \"type\": \"string\",\n      \"description\": \"The language code for results\"\n    },\n    \"regionCode\": {\n      \"type\": \"string\",\n      \"description\": \"The region code for biasing results\"\n    },\n    \"rankPreference\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"How results should be ranked\"\n    },\n    \"maxResultCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of results (1-20)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-search-nearby-request-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: SearchNearbyRequest
---
