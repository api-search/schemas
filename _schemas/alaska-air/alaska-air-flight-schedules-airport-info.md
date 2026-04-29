---
description: Airport served by Alaska Airlines
layout: schema
name: AirportInfo
properties_list:
- description: IATA airport code
  name: iataCode
  type: string
- description: Full airport name
  name: name
  type: string
- description: City name
  name: city
  type: string
- description: US state code
  name: state
  type: string
- description: ISO country code
  name: country
  type: string
- description: Airport latitude
  name: latitude
  type: number
- description: Airport longitude
  name: longitude
  type: number
- description: Airport timezone
  name: timezone
  type: string
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-flight-schedules-airport-info-schema.json
slug: alaska-air-flight-schedules-airport-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-schedules-airport-info-schema.json\",\n  \"title\": \"AirportInfo\",\n  \"description\": \"Airport served by Alaska Airlines\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iataCode\": {\n      \"type\": \"string\",\n      \"description\": \"IATA airport code\",\n      \"example\": \"SEA\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full airport name\",\n      \"example\": \"Seattle-Tacoma International Airport\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City name\",\n      \"example\": \"Seattle\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"US state code\",\n      \"example\": \"WA\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"ISO country\
  \ code\",\n      \"example\": \"US\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"description\": \"Airport latitude\",\n      \"example\": 47.4502\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"description\": \"Airport longitude\",\n      \"example\": -122.3088\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Airport timezone\",\n      \"example\": \"America/Los_Angeles\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-schedules-airport-info-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: AirportInfo
---
