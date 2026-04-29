---
description: A photo associated with a place
layout: schema
name: Photo
properties_list:
- description: The resource name of the photo in the format places/{placeId}/photos/{photoReference}
  name: name
  type: string
- description: Maximum available width in pixels
  name: widthPx
  type: integer
- description: Maximum available height in pixels
  name: heightPx
  type: integer
- description: The authors of this photo
  name: authorAttributions
  type: array
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-photo-schema.json
slug: google-maps-places-photo
source_filename: google-maps-places-photo-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Photo\",\n  \"type\": \"object\",\n  \"description\": \"A photo associated with a place\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the photo in the format places/{placeId}/photos/{photoReference}\"\n    },\n    \"widthPx\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum available width in pixels\"\n    },\n    \"heightPx\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum available height in pixels\"\n    },\n    \"authorAttributions\": {\n      \"type\": \"array\",\n      \"description\": \"The authors of this photo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-photo-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: Photo
---
