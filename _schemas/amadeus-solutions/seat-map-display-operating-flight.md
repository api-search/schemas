---
description: information about the operating flight
layout: schema
name: OperatingFlight
properties_list:
- description: providing the airline / carrier code
  name: carrierCode
  type: string
- description: the flight number as assigned by the carrier
  name: number
  type: string
- description: the flight number suffix as assigned by the carrier
  name: suffix
  type: string
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-operating-flight-schema.json
slug: seat-map-display-operating-flight
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-operating-flight-schema.json\",\n  \"title\": \"OperatingFlight\",\n  \"description\": \"information about the operating flight\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"carrierCode\": {\n      \"type\": \"string\",\n      \"description\": \"providing the airline / carrier code\",\n      \"minLength\": 1,\n      \"maxLength\": 2,\n      \"example\": \"DL\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"the flight number as assigned by the carrier\",\n      \"minLength\": 1,\n      \"maxLength\": 4,\n      \"example\": \"212\"\n    },\n    \"suffix\": {\n      \"type\": \"string\",\n      \"description\": \"the flight number suffix as assigned by the carrier\",\n      \"minLength\": 1,\n      \"maxLength\": 4\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-operating-flight-schema.json
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
