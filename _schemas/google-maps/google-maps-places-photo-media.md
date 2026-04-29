---
description: Photo media metadata returned when skipHttpRedirect is true
layout: schema
name: PhotoMedia
properties_list:
- description: The resource name of the photo media
  name: name
  type: string
- description: A short-lived URI for the photo
  name: photoUri
  type: string
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-photo-media-schema.json
slug: google-maps-places-photo-media
source_filename: google-maps-places-photo-media-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PhotoMedia\",\n  \"type\": \"object\",\n  \"description\": \"Photo media metadata returned when skipHttpRedirect is true\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the photo media\"\n    },\n    \"photoUri\": {\n      \"type\": \"string\",\n      \"description\": \"A short-lived URI for the photo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-photo-media-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: PhotoMedia
---
