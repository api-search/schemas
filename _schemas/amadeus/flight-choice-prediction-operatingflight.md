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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-choice-prediction-operatingflight-schema.json
slug: flight-choice-prediction-operatingflight
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"OperatingFlight\",\n  \"description\": \"information about the operating flight\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"carrierCode\": {\n      \"type\": \"string\",\n      \"description\": \"providing the airline / carrier code\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"the flight number as assigned by the carrier\"\n    },\n    \"suffix\": {\n      \"type\": \"string\",\n      \"description\": \"the flight number suffix as assigned by the carrier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-choice-prediction-operatingflight-schema.json
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
title: OperatingFlight
---
