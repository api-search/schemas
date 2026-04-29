---
description: ''
layout: schema
name: flightDesignator
properties_list:
- description: Two letter IATA standard carrier code
  name: carrierCode
  type: string
- description: 1-4 digit number
  name: flightNumber
  type: string
- description: the operational suffix
  name: operationalSuffix
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-flightdesignator-schema.json
slug: trip-parser-flightdesignator
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"flightDesignator\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"carrierCode\": {\n      \"type\": \"string\",\n      \"description\": \"Two letter IATA standard carrier code\"\n    },\n    \"flightNumber\": {\n      \"type\": \"string\",\n      \"description\": \"1-4 digit number\"\n    },\n    \"operationalSuffix\": {\n      \"type\": \"string\",\n      \"description\": \"the operational suffix\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-flightdesignator-schema.json
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
title: flightDesignator
---
