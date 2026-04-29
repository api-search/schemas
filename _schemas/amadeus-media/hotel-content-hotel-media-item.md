---
description: A detailed media item with dimensions and format information.
layout: schema
name: HotelMediaItem
properties_list:
- description: Unique identifier for the media item.
  name: id
  type: string
- description: Media category type.
  name: category
  type: string
- description: URL of the full-size image.
  name: uri
  type: string
- description: URL of the thumbnail image.
  name: thumbnailUri
  type: string
- description: Image caption or alt text.
  name: caption
  type: string
- description: Image width in pixels.
  name: width
  type: integer
- description: Image height in pixels.
  name: height
  type: integer
- description: Image format.
  name: format
  type: string
- description: Indicates whether this is the primary/featured image for this category.
  name: isPrimary
  type: boolean
provider_name: Amadeus Media
provider_slug: amadeus-media
schema_file: json-schema/hotel-content-hotel-media-item-schema.json
slug: hotel-content-hotel-media-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-media-item-schema.json\",\n  \"title\": \"HotelMediaItem\",\n  \"description\": \"A detailed media item with dimensions and format information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the media item.\",\n      \"example\": \"media-001\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Media category type.\",\n      \"example\": \"EXTERIOR\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the full-size image.\",\n      \"example\": \"https://media.amadeus.com/hotels/MCLONGHM/exterior-01.jpg\"\n    },\n    \"thumbnailUri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n    \
  \  \"description\": \"URL of the thumbnail image.\",\n      \"example\": \"https://media.amadeus.com/hotels/MCLONGHM/exterior-01-thumb.jpg\"\n    },\n    \"caption\": {\n      \"type\": \"string\",\n      \"description\": \"Image caption or alt text.\",\n      \"example\": \"Hotel Exterior View\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Image width in pixels.\",\n      \"example\": 1920\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"Image height in pixels.\",\n      \"example\": 1080\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"Image format.\",\n      \"enum\": [\n        \"JPEG\",\n        \"PNG\",\n        \"WEBP\"\n      ],\n      \"example\": \"JPEG\"\n    },\n    \"isPrimary\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this is the primary/featured image for this category.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-media-item-schema.json
tags:
- Content
- Hotels
- Images
- Media
- Travel
title: HotelMediaItem
---
