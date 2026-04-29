---
description: Media assets for a single hotel.
layout: schema
name: HotelMediaData
properties_list:
- description: Amadeus property code.
  name: hotelId
  type: string
- description: List of media assets for the hotel.
  name: media
  type: array
provider_name: Amadeus Media
provider_slug: amadeus-media
schema_file: json-schema/hotel-content-hotel-media-data-schema.json
slug: hotel-content-hotel-media-data
source_filename: hotel-content-hotel-media-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-media-data-schema.json\",\n  \"title\": \"HotelMediaData\",\n  \"description\": \"Media assets for a single hotel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hotelId\": {\n      \"type\": \"string\",\n      \"description\": \"Amadeus property code.\",\n      \"example\": \"MCLONGHM\"\n    },\n    \"media\": {\n      \"type\": \"array\",\n      \"description\": \"List of media assets for the hotel.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/HotelMediaItem\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-media-data-schema.json
tags:
- Content
- Hotels
- Images
- Media
- Travel
title: HotelMediaData
---
