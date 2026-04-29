---
description: FlightList schema
layout: schema
name: FlightList
properties_list:
- description: ''
  name: flights
  type: array
provider_name: American Airlines
provider_slug: american-airlines
schema_file: json-schema/runway-developer-api-flight-list-schema.json
slug: runway-developer-api-flight-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/american-airlines/refs/heads/main/json-schema/runway-developer-api-flight-list-schema.json\",\n  \"title\": \"FlightList\",\n  \"description\": \"FlightList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flights\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Flight\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/american-airlines/refs/heads/main/json-schema/runway-developer-api-flight-list-schema.json
tags:
- Airlines
- Aviation
- Flights
- Travel
- Booking
- Developer Experience
title: FlightList
---
