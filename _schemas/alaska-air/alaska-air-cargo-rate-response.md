---
description: Cargo rate estimate response
layout: schema
name: RateResponse
properties_list:
- description: Origin airport IATA code
  name: origin
  type: string
- description: Destination airport IATA code
  name: destination
  type: string
- description: Ship date
  name: shipDate
  type: string
- description: Estimated total charge
  name: totalCharge
  type: number
- description: Currency code
  name: currency
  type: string
- description: Rate per kilogram
  name: ratePerKg
  type: number
- description: Estimated transit days
  name: transitDays
  type: integer
- description: Service type
  name: serviceType
  type: string
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-cargo-rate-response-schema.json
slug: alaska-air-cargo-rate-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-cargo-rate-response-schema.json\",\n  \"title\": \"RateResponse\",\n  \"description\": \"Cargo rate estimate response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"origin\": {\n      \"type\": \"string\",\n      \"description\": \"Origin airport IATA code\",\n      \"example\": \"SEA\"\n    },\n    \"destination\": {\n      \"type\": \"string\",\n      \"description\": \"Destination airport IATA code\",\n      \"example\": \"HNL\"\n    },\n    \"shipDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Ship date\",\n      \"example\": \"2026-04-20\"\n    },\n    \"totalCharge\": {\n      \"type\": \"number\",\n      \"description\": \"Estimated total charge\",\n      \"example\": 385.5\n    },\n    \"currency\": {\n      \"type\": \"string\",\n  \
  \    \"description\": \"Currency code\",\n      \"example\": \"USD\"\n    },\n    \"ratePerKg\": {\n      \"type\": \"number\",\n      \"description\": \"Rate per kilogram\",\n      \"example\": 8.47\n    },\n    \"transitDays\": {\n      \"type\": \"integer\",\n      \"description\": \"Estimated transit days\",\n      \"example\": 1\n    },\n    \"serviceType\": {\n      \"type\": \"string\",\n      \"description\": \"Service type\",\n      \"example\": \"Standard\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-cargo-rate-response-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: RateResponse
---
