---
description: Vehicle describes the transportation means e.g. a Train, a Bus, etc. It may be further characterized, in the case of a Train, it contains the Train Number, Code etc.
layout: schema
name: vehicle
properties_list:
- description: Code (codelist TVT) for the generic transport service returned, e.g. High speed, Intercities, Night and so on
  name: vehicleType
  type: string
- description: ''
  name: code
  type: string
- description: ''
  name: number
  type: string
- description: ''
  name: displayName
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-vehicle-schema.json
slug: trip-parser-vehicle
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"vehicle\",\n  \"description\": \"Vehicle describes the transportation means e.g. a Train, a Bus, etc. It may be further characterized, in the case of a Train, it contains the Train Number, Code etc.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicleType\": {\n      \"type\": \"string\",\n      \"description\": \"Code (codelist TVT) for the generic transport service returned, e.g. High speed, Intercities, Night and so on\"\n    },\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"number\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-vehicle-schema.json
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
title: vehicle
---
