---
description: Detailed content for a single hotel property.
layout: schema
name: HotelContent
properties_list:
- description: Amadeus property code (8 characters).
  name: hotelId
  type: string
- description: Hotel chain code.
  name: chainCode
  type: string
- description: IATA city code where the hotel is located.
  name: iataCode
  type: string
- description: Hotel name.
  name: name
  type: string
- description: ''
  name: basicInfo
  type: object
- description: Hotel descriptions in various languages.
  name: descriptions
  type: array
- description: ''
  name: contact
  type: object
- description: ''
  name: address
  type: object
- description: ''
  name: geoCode
  type: object
- description: List of hotel amenity codes.
  name: amenities
  type: array
- description: List of hotel media assets.
  name: media
  type: array
provider_name: Amadeus Media
provider_slug: amadeus-media
schema_file: json-schema/hotel-content-hotel-content-schema.json
slug: hotel-content-hotel-content
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-content-schema.json\",\n  \"title\": \"HotelContent\",\n  \"description\": \"Detailed content for a single hotel property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hotelId\": {\n      \"type\": \"string\",\n      \"description\": \"Amadeus property code (8 characters).\",\n      \"example\": \"MCLONGHM\"\n    },\n    \"chainCode\": {\n      \"type\": \"string\",\n      \"description\": \"Hotel chain code.\",\n      \"example\": \"MC\"\n    },\n    \"iataCode\": {\n      \"type\": \"string\",\n      \"description\": \"IATA city code where the hotel is located.\",\n      \"example\": \"LON\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Hotel name.\",\n      \"example\": \"THE LONGCHAMP HOTEL\"\n    },\n    \"basicInfo\": {\n      \"$ref\"\
  : \"#/components/schemas/HotelBasicInfo\"\n    },\n    \"descriptions\": {\n      \"type\": \"array\",\n      \"description\": \"Hotel descriptions in various languages.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/HotelDescription\"\n      }\n    },\n    \"contact\": {\n      \"$ref\": \"#/components/schemas/HotelContact\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/HotelAddress\"\n    },\n    \"geoCode\": {\n      \"$ref\": \"#/components/schemas/GeoCode\"\n    },\n    \"amenities\": {\n      \"type\": \"array\",\n      \"description\": \"List of hotel amenity codes.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"WIFI\",\n        \"RESTAURANT\",\n        \"SPA\"\n      ]\n    },\n    \"media\": {\n      \"type\": \"array\",\n      \"description\": \"List of hotel media assets.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MediaAsset\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-content-schema.json
tags:
- Content
- Hotels
- Images
- Media
- Travel
title: HotelContent
---
