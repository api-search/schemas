---
description: Response from the autocomplete endpoint
layout: schema
name: AutocompleteResponse
properties_list:
- description: List of autocomplete suggestions
  name: suggestions
  type: array
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-autocomplete-response-schema.json
slug: google-maps-places-autocomplete-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AutocompleteResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response from the autocomplete endpoint\",\n  \"properties\": {\n    \"suggestions\": {\n      \"type\": \"array\",\n      \"description\": \"List of autocomplete suggestions\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-autocomplete-response-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: AutocompleteResponse
---
