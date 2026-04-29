---
description: BookingRequest schema
layout: schema
name: BookingRequest
properties_list:
- description: ''
  name: flightId
  type: string
- description: ''
  name: passengers
  type: array
provider_name: American Airlines
provider_slug: american-airlines
schema_file: json-schema/runway-developer-api-booking-request-schema.json
slug: runway-developer-api-booking-request
source_filename: runway-developer-api-booking-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/american-airlines/refs/heads/main/json-schema/runway-developer-api-booking-request-schema.json\",\n  \"title\": \"BookingRequest\",\n  \"description\": \"BookingRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flightId\": {\n      \"type\": \"string\"\n    },\n    \"passengers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"firstName\": {\n            \"type\": \"string\"\n          },\n          \"lastName\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/american-airlines/refs/heads/main/json-schema/runway-developer-api-booking-request-schema.json
tags:
- Airlines
- Aviation
- Flights
- Travel
- Booking
- Developer Experience
title: BookingRequest
---
