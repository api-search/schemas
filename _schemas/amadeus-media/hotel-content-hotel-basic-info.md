---
description: Basic hotel classification information.
layout: schema
name: HotelBasicInfo
properties_list:
- description: Hotel star category (1-5).
  name: category
  type: integer
- description: Hotel rating classification.
  name: rating
  type: string
- description: Total number of rooms in the property.
  name: numberOfRooms
  type: integer
- description: Standard check-in time (HH:MM format).
  name: checkInTime
  type: string
- description: Standard check-out time (HH:MM format).
  name: checkOutTime
  type: string
provider_name: Amadeus Media
provider_slug: amadeus-media
schema_file: json-schema/hotel-content-hotel-basic-info-schema.json
slug: hotel-content-hotel-basic-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-basic-info-schema.json\",\n  \"title\": \"HotelBasicInfo\",\n  \"description\": \"Basic hotel classification information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"integer\",\n      \"description\": \"Hotel star category (1-5).\",\n      \"example\": 4\n    },\n    \"rating\": {\n      \"type\": \"string\",\n      \"description\": \"Hotel rating classification.\",\n      \"example\": \"FOUR_STARS\"\n    },\n    \"numberOfRooms\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of rooms in the property.\",\n      \"example\": 120\n    },\n    \"checkInTime\": {\n      \"type\": \"string\",\n      \"description\": \"Standard check-in time (HH:MM format).\",\n      \"example\": \"14:00\"\n    },\n    \"checkOutTime\":\
  \ {\n      \"type\": \"string\",\n      \"description\": \"Standard check-out time (HH:MM format).\",\n      \"example\": \"12:00\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-basic-info-schema.json
tags:
- Content
- Hotels
- Images
- Media
- Travel
title: HotelBasicInfo
---
