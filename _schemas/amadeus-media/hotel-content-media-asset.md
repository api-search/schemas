---
description: A single media asset (image or video) for a hotel property.
layout: schema
name: MediaAsset
properties_list:
- description: Media category.
  name: category
  type: string
- description: URL of the full-size media asset.
  name: uri
  type: string
- description: Caption or alt text for the media asset.
  name: caption
  type: string
provider_name: Amadeus Media
provider_slug: amadeus-media
schema_file: json-schema/hotel-content-media-asset-schema.json
slug: hotel-content-media-asset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-media-asset-schema.json\",\n  \"title\": \"MediaAsset\",\n  \"description\": \"A single media asset (image or video) for a hotel property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Media category.\",\n      \"enum\": [\n        \"EXTERIOR\",\n        \"LOBBY\",\n        \"ROOM\",\n        \"RESTAURANT\",\n        \"POOL\",\n        \"SPA\",\n        \"GYM\",\n        \"MEETING_ROOM\",\n        \"COMMON_AREA\"\n      ],\n      \"example\": \"EXTERIOR\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the full-size media asset.\",\n      \"example\": \"https://media.amadeus.com/hotels/MCLONGHM/exterior-01.jpg\"\n    },\n    \"caption\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Caption or alt text for the media asset.\",\n      \"example\": \"Hotel Exterior\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-media-asset-schema.json
tags:
- Content
- Hotels
- Images
- Media
- Travel
title: MediaAsset
---
