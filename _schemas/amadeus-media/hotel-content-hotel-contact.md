---
description: Hotel contact information.
layout: schema
name: HotelContact
properties_list:
- description: Hotel phone number in international format.
  name: phone
  type: string
- description: Hotel fax number.
  name: fax
  type: string
- description: Hotel email address.
  name: email
  type: string
- description: Hotel website URL.
  name: website
  type: string
provider_name: Amadeus Media
provider_slug: amadeus-media
schema_file: json-schema/hotel-content-hotel-contact-schema.json
slug: hotel-content-hotel-contact
source_filename: hotel-content-hotel-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-contact-schema.json\",\n  \"title\": \"HotelContact\",\n  \"description\": \"Hotel contact information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Hotel phone number in international format.\",\n      \"example\": \"+44-20-12345678\"\n    },\n    \"fax\": {\n      \"type\": \"string\",\n      \"description\": \"Hotel fax number.\",\n      \"example\": \"+44-20-12345679\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Hotel email address.\",\n      \"example\": \"info@hotel.com\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Hotel website URL.\",\n      \"example\": \"https://www.hotel.com\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/json-schema/hotel-content-hotel-contact-schema.json
tags:
- Content
- Hotels
- Images
- Media
- Travel
title: HotelContact
---
