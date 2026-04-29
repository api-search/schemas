---
description: PassengerCharacteristics schema
layout: schema
name: PassengerCharacteristics
properties_list:
- description: Passenger type codes e.g. CHD , ADT. CHD is for child and ADT for Adult.
  name: passengerTypeCode
  type: string
- description: Age of the Passenger (Mandatory if typeCode= “CHD”)
  name: age
  type: integer
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-passenger-characteristics-schema.json
slug: transfer-booking-passenger-characteristics
source_filename: transfer-booking-passenger-characteristics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-passenger-characteristics-schema.json\",\n  \"title\": \"PassengerCharacteristics\",\n  \"description\": \"PassengerCharacteristics schema\",\n  \"properties\": {\n    \"passengerTypeCode\": {\n      \"description\": \"Passenger type codes e.g. CHD , ADT. CHD is for child and ADT for Adult.\",\n      \"type\": \"string\",\n      \"example\": \"child\"\n    },\n    \"age\": {\n      \"type\": \"integer\",\n      \"description\": \"Age of the Passenger (Mandatory if typeCode= \\u201cCHD\\u201d)\",\n      \"example\": 12\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-passenger-characteristics-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: PassengerCharacteristics
---
