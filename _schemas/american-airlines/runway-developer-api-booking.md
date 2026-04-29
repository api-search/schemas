---
description: Booking schema
layout: schema
name: Booking
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: flightId
  type: string
- description: ''
  name: passengers
  type: array
- description: ''
  name: status
  type: string
provider_name: American Airlines
provider_slug: american-airlines
schema_file: json-schema/runway-developer-api-booking-schema.json
slug: runway-developer-api-booking
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/american-airlines/refs/heads/main/json-schema/runway-developer-api-booking-schema.json\",\n  \"title\": \"Booking\",\n  \"description\": \"Booking schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"flightId\": {\n      \"type\": \"string\"\n    },\n    \"passengers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"seatNumber\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/american-airlines/refs/heads/main/json-schema/runway-developer-api-booking-schema.json
tags:
- Airlines
- Aviation
- Flights
- Travel
- Booking
- Developer Experience
title: Booking
---
