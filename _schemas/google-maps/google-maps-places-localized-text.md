---
description: A localized text string
layout: schema
name: LocalizedText
properties_list:
- description: The localized text value
  name: text
  type: string
- description: BCP-47 language code of the text
  name: languageCode
  type: string
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-localized-text-schema.json
slug: google-maps-places-localized-text
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LocalizedText\",\n  \"type\": \"object\",\n  \"description\": \"A localized text string\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The localized text value\"\n    },\n    \"languageCode\": {\n      \"type\": \"string\",\n      \"description\": \"BCP-47 language code of the text\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-localized-text-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: LocalizedText
---
