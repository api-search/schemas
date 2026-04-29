---
description: Hotel description in a specific language.
layout: schema
name: HotelDescription
properties_list:
- description: ISO 639-1 language code.
  name: lang
  type: string
- description: Hotel description text.
  name: text
  type: string
provider_name: Amadeus Media
provider_slug: amadeus-media
schema_file: json-schema/hotel-content-hotel-description-schema.json
slug: hotel-content-hotel-description
source_filename: hotel-content-hotel-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-description-schema.json\",\n  \"title\": \"HotelDescription\",\n  \"description\": \"Hotel description in a specific language.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lang\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 639-1 language code.\",\n      \"example\": \"EN\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Hotel description text.\",\n      \"example\": \"A luxury boutique hotel offering exceptional service and stunning city views.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-description-schema.json
tags:
- Content
- Hotels
- Images
- Media
- Travel
title: HotelDescription
---
