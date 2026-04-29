---
description: ''
layout: schema
name: Dictionaries
properties_list:
- description: ''
  name: locations
  type: object
- description: ''
  name: aircraft
  type: object
- description: ''
  name: currencies
  type: object
- description: ''
  name: carriers
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-order-management-dictionaries-schema.json
slug: flight-order-management-dictionaries
source_filename: flight-order-management-dictionaries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Dictionaries\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"locations\": {\n      \"$ref\": \"#/definitions/LocationEntry\"\n    },\n    \"aircraft\": {\n      \"$ref\": \"#/definitions/AircraftEntry\"\n    },\n    \"currencies\": {\n      \"$ref\": \"#/definitions/CurrencyEntry\"\n    },\n    \"carriers\": {\n      \"$ref\": \"#/definitions/CarrierEntry\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-order-management-dictionaries-schema.json
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
title: Dictionaries
---
