---
description: stakeholder definition
layout: schema
name: Stakeholder
properties_list:
- description: item identifier
  name: id
  type: string
- description: The date of birth in ISO 8601 format (yyyy-mm-dd)
  name: dateOfBirth
  type: string
- description: ''
  name: gender
  type: object
- description: ''
  name: name
  type: object
- description: Advanced Passenger Information - regulatory identity documents - SSR DOCS & DOCO elements
  name: documents
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-create-orders-stakeholder-schema.json
slug: flight-create-orders-stakeholder
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Stakeholder\",\n  \"description\": \"stakeholder definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"item identifier\"\n    },\n    \"dateOfBirth\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date of birth in ISO 8601 format (yyyy-mm-dd)\"\n    },\n    \"gender\": {\n      \"$ref\": \"#/definitions/StakeholderGender\"\n    },\n    \"name\": {\n      \"$ref\": \"#/definitions/Name\"\n    },\n    \"documents\": {\n      \"type\": \"array\",\n      \"description\": \"Advanced Passenger Information - regulatory identity documents - SSR DOCS & DOCO elements\",\n      \"items\": {\n        \"$ref\": \"#/definitions/IdentityDocument\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-create-orders-stakeholder-schema.json
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
title: Stakeholder
---
