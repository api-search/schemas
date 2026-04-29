---
description: ''
layout: schema
name: FlightDesignator
properties_list:
- description: 2 to 3-character IATA code of the carrier. e.g. 6X
  name: carrierCode
  type: string
- description: 1 to 4-digit number of the flight e.g. 4537
  name: flightNumber
  type: integer
- description: 1-letter operational suffix of the flight e.g. A
  name: operationalSuffix
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/on-demand-flight-status-flightdesignator-schema.json
slug: on-demand-flight-status-flightdesignator
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FlightDesignator\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"carrierCode\": {\n      \"type\": \"string\",\n      \"description\": \"2 to 3-character IATA code of the carrier. e.g. 6X\"\n    },\n    \"flightNumber\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"1 to 4-digit number of the flight e.g. 4537\"\n    },\n    \"operationalSuffix\": {\n      \"type\": \"string\",\n      \"description\": \"1-letter operational suffix of the flight e.g. A\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/on-demand-flight-status-flightdesignator-schema.json
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
title: FlightDesignator
---
