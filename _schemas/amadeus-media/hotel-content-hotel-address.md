---
description: Hotel physical address.
layout: schema
name: HotelAddress
properties_list:
- description: Street address lines.
  name: lines
  type: array
- description: Postal or ZIP code.
  name: postalCode
  type: string
- description: City name.
  name: cityName
  type: string
- description: ISO 3166-1 alpha-2 country code.
  name: countryCode
  type: string
- description: State or province code (where applicable).
  name: stateCode
  type: string
provider_name: Amadeus Media
provider_slug: amadeus-media
schema_file: json-schema/hotel-content-hotel-address-schema.json
slug: hotel-content-hotel-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-address-schema.json\",\n  \"title\": \"HotelAddress\",\n  \"description\": \"Hotel physical address.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lines\": {\n      \"type\": \"array\",\n      \"description\": \"Street address lines.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"15 Park Lane\"\n      ]\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal or ZIP code.\",\n      \"example\": \"W1K 1BE\"\n    },\n    \"cityName\": {\n      \"type\": \"string\",\n      \"description\": \"City name.\",\n      \"example\": \"London\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code.\",\n      \"example\": \"GB\"\n    },\n \
  \   \"stateCode\": {\n      \"type\": \"string\",\n      \"description\": \"State or province code (where applicable).\",\n      \"example\": \"ENG\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-address-schema.json
tags:
- Content
- Hotels
- Images
- Media
- Travel
title: HotelAddress
---
