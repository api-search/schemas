---
description: Information about the author of a review
layout: schema
name: AuthorAttribution
properties_list:
- description: Name of the review author
  name: displayName
  type: string
- description: URI of the author's profile
  name: uri
  type: string
- description: URI of the author's profile photo
  name: photoUri
  type: string
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-author-attribution-schema.json
slug: google-maps-places-author-attribution
source_filename: google-maps-places-author-attribution-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AuthorAttribution\",\n  \"type\": \"object\",\n  \"description\": \"Information about the author of a review\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the review author\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the author's profile\"\n    },\n    \"photoUri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the author's profile photo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-author-attribution-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: AuthorAttribution
---
