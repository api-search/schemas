---
description: Price schema
layout: schema
name: Price
properties_list:
- description: ''
  name: currency
  type: string
- description: Total amount paid by the user
  name: total
  type: string
- description: Amount without taxes
  name: base
  type: string
- description: List of applicable fees
  name: fees
  type: array
- description: ''
  name: taxes
  type: array
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-price-schema.json
slug: seat-map-display-price
source_filename: seat-map-display-price-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-price-schema.json\",\n  \"title\": \"Price\",\n  \"description\": \"Price schema\",\n  \"properties\": {\n    \"currency\": {\n      \"type\": \"string\",\n      \"example\": \"USD\"\n    },\n    \"total\": {\n      \"description\": \"Total amount paid by the user\",\n      \"type\": \"string\",\n      \"example\": \"932.70\"\n    },\n    \"base\": {\n      \"description\": \"Amount without taxes\",\n      \"type\": \"string\",\n      \"example\": \"632.70\"\n    },\n    \"fees\": {\n      \"description\": \"List of applicable fees\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Fee\"\n      }\n    },\n    \"taxes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Tax\"\n      }\n    }\n  },\n  \"type\": \"object\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-price-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Price
---
