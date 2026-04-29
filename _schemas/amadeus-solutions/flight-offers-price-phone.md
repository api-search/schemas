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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-phone-schema.json
slug: flight-offers-price-phone
source_filename: flight-offers-price-phone-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-phone-schema.json\",\n  \"title\": \"Phone\",\n  \"description\": \"phone information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deviceType\": {\n      \"$ref\": \"#/definitions/PhoneDeviceType\"\n    },\n    \"countryCallingCode\": {\n      \"type\": \"string\",\n      \"description\": \"Country calling code of the phone number, as defined by the International Communication Union. Examples - \\\"1\\\" for US, \\\"371\\\" for Latvia.\",\n      \"pattern\": \"[0-9+]{2,5}\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number. Composed of digits only. The number of digits depends on the country.\",\n      \"pattern\": \"[0-9]{1,15}\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-phone-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Phone
---
