---
description: Dictionaries schema
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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/branded-fares-upsell-dictionaries-schema.json
slug: branded-fares-upsell-dictionaries
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-dictionaries-schema.json\",\n  \"title\": \"Dictionaries\",\n  \"description\": \"Dictionaries schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"locations\": {\n      \"$ref\": \"#/definitions/LocationEntry\"\n    },\n    \"aircraft\": {\n      \"$ref\": \"#/definitions/AircraftEntry\"\n    },\n    \"currencies\": {\n      \"$ref\": \"#/definitions/CurrencyEntry\"\n    },\n    \"carriers\": {\n      \"$ref\": \"#/definitions/CarrierEntry\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-dictionaries-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Dictionaries
---
