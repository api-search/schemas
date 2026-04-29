---
description: information about the operating flight
layout: schema
name: OperatingFlight
properties_list:
- description: providing the airline / carrier code
  name: carrierCode
  type: string
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-operating-flight-schema.json
slug: flight-offers-price-operating-flight
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-operating-flight-schema.json\",\n  \"title\": \"OperatingFlight\",\n  \"description\": \"information about the operating flight\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"carrierCode\": {\n      \"type\": \"string\",\n      \"description\": \"providing the airline / carrier code\",\n      \"minLength\": 1,\n      \"maxLength\": 2,\n      \"example\": \"DL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-operating-flight-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: OperatingFlight
---
