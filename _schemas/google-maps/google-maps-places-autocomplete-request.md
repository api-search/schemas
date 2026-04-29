---
description: Request body for place autocomplete predictions
layout: schema
name: AutocompleteRequest
properties_list:
- description: The text input specifying which place to search for
  name: input
  type: string
- description: Restrict results to primary types
  name: includedPrimaryTypes
  type: array
- description: Restrict results to these region codes
  name: includedRegionCodes
  type: array
- description: The language code for predictions
  name: languageCode
  type: string
- description: Region code for biasing
  name: regionCode
  type: string
- description: Zero-based Unicode character offset of input indicating the cursor position. Use to return more relevant predictions.
  name: inputOffset
  type: integer
- description: Whether to include query predictions in results
  name: includeQueryPredictions
  type: boolean
- description: A random string that groups this request with subsequent Place Details requests for billing.
  name: sessionToken
  type: string
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-autocomplete-request-schema.json
slug: google-maps-places-autocomplete-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AutocompleteRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for place autocomplete predictions\",\n  \"properties\": {\n    \"input\": {\n      \"type\": \"string\",\n      \"description\": \"The text input specifying which place to search for\"\n    },\n    \"includedPrimaryTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Restrict results to primary types\"\n    },\n    \"includedRegionCodes\": {\n      \"type\": \"array\",\n      \"description\": \"Restrict results to these region codes\"\n    },\n    \"languageCode\": {\n      \"type\": \"string\",\n      \"description\": \"The language code for predictions\"\n    },\n    \"regionCode\": {\n      \"type\": \"string\",\n      \"description\": \"Region code for biasing\"\n    },\n    \"inputOffset\": {\n      \"type\": \"integer\",\n      \"description\": \"Zero-based Unicode character offset of input\
  \ indicating the cursor position. Use to return more relevant predictions.\"\n    },\n    \"includeQueryPredictions\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include query predictions in results\"\n    },\n    \"sessionToken\": {\n      \"type\": \"string\",\n      \"description\": \"A random string that groups this request with subsequent Place Details requests for billing.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-autocomplete-request-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: AutocompleteRequest
---
