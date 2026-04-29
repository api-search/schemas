---
description: the traveler of the trip
layout: schema
name: Traveler
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-traveler-schema.json
slug: flight-order-management-traveler
source_filename: flight-order-management-traveler-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-traveler-schema.json\",\n  \"title\": \"Traveler\",\n  \"description\": \"the traveler of the trip\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/Stakeholder\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"emergencyContact\": {\n          \"description\": \"emergency contact\",\n          \"$ref\": \"#/definitions/EmergencyContact\"\n        },\n        \"loyaltyPrograms\": {\n          \"description\": \"list of loyalty program followed by the traveler\",\n          \"type\": \"array\",\n          \"minItems\": 0,\n          \"maxItems\": 10,\n          \"items\": {\n            \"$ref\": \"#/definitions/LoyaltyProgram\"\n          }\n        },\n        \"discountEligibility\": {\n          \"description\": \"list of element that\
  \ allow a discount.\",\n          \"type\": \"array\",\n          \"minItems\": 0,\n          \"maxItems\": 10,\n          \"items\": {\n            \"$ref\": \"#/definitions/Discount\"\n          }\n        },\n        \"contact\": {\n          \"$ref\": \"#/definitions/Contact\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-traveler-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Traveler
---
