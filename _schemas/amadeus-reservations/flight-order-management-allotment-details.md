---
description: AllotmentDetails schema
layout: schema
name: AllotmentDetails
properties_list:
- description: The tour name agreed for this specific allotment.
  name: tourName
  type: string
- description: The tour reference agreed for this specific allotment.
  name: tourReference
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-allotment-details-schema.json
slug: flight-order-management-allotment-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-allotment-details-schema.json\",\n  \"title\": \"AllotmentDetails\",\n  \"description\": \"AllotmentDetails schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tourName\": {\n      \"description\": \"The tour name agreed for this specific allotment.\",\n      \"type\": \"string\"\n    },\n    \"tourReference\": {\n      \"description\": \"The tour reference agreed for this specific allotment.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-allotment-details-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: AllotmentDetails
---
