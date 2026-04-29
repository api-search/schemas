---
description: ''
layout: schema
name: PassengerCharacteristics
properties_list:
- description: Passenger type codes e.g. CHD , ADT. CHD is for child and ADT for Adult.
  name: passengerTypeCode
  type: string
- description: Age of the Passenger (Mandatory if typeCode= “CHD”)
  name: age
  type: integer
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-search-passengercharacteristics-schema.json
slug: transfer-search-passengercharacteristics
source_filename: transfer-search-passengercharacteristics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"PassengerCharacteristics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"passengerTypeCode\": {\n      \"type\": \"string\",\n      \"description\": \"Passenger type codes e.g. CHD , ADT. CHD is for child and ADT for Adult.\"\n    },\n    \"age\": {\n      \"type\": \"integer\",\n      \"description\": \"Age of the Passenger (Mandatory if typeCode= \\u201cCHD\\u201d)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-search-passengercharacteristics-schema.json
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: PassengerCharacteristics
---
