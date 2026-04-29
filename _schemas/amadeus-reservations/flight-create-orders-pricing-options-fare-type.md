---
description: type of fare of the flight-offer
layout: schema
name: PricingOptionsFareType
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-pricing-options-fare-type-schema.json
slug: flight-create-orders-pricing-options-fare-type
source_filename: flight-create-orders-pricing-options-fare-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-pricing-options-fare-type-schema.json\",\n  \"title\": \"PricingOptionsFareType\",\n  \"description\": \"type of fare of the flight-offer\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"enum\": [\n      \"PUBLISHED\"\n    ]\n  },\n  \"example\": [\n    \"PUBLISHED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-pricing-options-fare-type-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: PricingOptionsFareType
---
