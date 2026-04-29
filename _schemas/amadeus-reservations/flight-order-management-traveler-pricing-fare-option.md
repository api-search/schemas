---
description: option specifying a group of fares, which may be valid under certain conditons Can be used to specify special fare discount for a passenger
layout: schema
name: TravelerPricingFareOption
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-traveler-pricing-fare-option-schema.json
slug: flight-order-management-traveler-pricing-fare-option
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-traveler-pricing-fare-option-schema.json\",\n  \"title\": \"TravelerPricingFareOption\",\n  \"description\": \"option specifying a group of fares, which may be valid under certain conditons\\nCan be used to specify special fare discount for a passenger\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"STANDARD\",\n    \"INCLUSIVE_TOUR\",\n    \"SPANISH_MELILLA_RESIDENT\",\n    \"SPANISH_CEUTA_RESIDENT\",\n    \"SPANISH_CANARY_RESIDENT\",\n    \"SPANISH_BALEARIC_RESIDENT\",\n    \"AIR_FRANCE_METROPOLITAN_DISCOUNT_PASS\",\n    \"AIR_FRANCE_DOM_DISCOUNT_PASS\",\n    \"AIR_FRANCE_COMBINED_DISCOUNT_PASS\",\n    \"AIR_FRANCE_FAMILY\",\n    \"ADULT_WITH_COMPANION\",\n    \"COMPANION\"\n  ],\n  \"example\": \"STANDARD\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-traveler-pricing-fare-option-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: TravelerPricingFareOption
---
