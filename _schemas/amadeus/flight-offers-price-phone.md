---
description: phone information
layout: schema
name: Phone
properties_list:
- description: ''
  name: deviceType
  type: object
- description: Country calling code of the phone number, as defined by the International Communication Union. Examples - "1" for US, "371" for Latvia.
  name: countryCallingCode
  type: string
- description: Phone number. Composed of digits only. The number of digits depends on the country.
  name: number
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-price-phone-schema.json
slug: flight-offers-price-phone
source_filename: flight-offers-price-phone-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Phone\",\n  \"description\": \"phone information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deviceType\": {\n      \"$ref\": \"#/definitions/PhoneDeviceType\"\n    },\n    \"countryCallingCode\": {\n      \"type\": \"string\",\n      \"description\": \"Country calling code of the phone number, as defined by the International Communication Union. Examples - \\\"1\\\" for US, \\\"371\\\" for Latvia.\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number. Composed of digits only. The number of digits depends on the country.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-price-phone-schema.json
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
title: Phone
---
