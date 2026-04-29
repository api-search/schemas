---
description: fare filter options
layout: schema
name: ExtendedPricingOptions
properties_list:
- description: If true, returns the flight-offers with included checked bags only
  name: includedCheckedBagsOnly
  type: boolean
- description: If true, returns the flight-offers with refundable fares only
  name: refundableFare
  type: boolean
- description: If true, returns the flight-offers with no restriction fares only
  name: noRestrictionFare
  type: boolean
- description: If true, returns the flight-offers with no penalty fares only
  name: noPenaltyFare
  type: boolean
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-search-extendedpricingoptions-schema.json
slug: flight-offers-search-extendedpricingoptions
source_filename: flight-offers-search-extendedpricingoptions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ExtendedPricingOptions\",\n  \"description\": \"fare filter options\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"includedCheckedBagsOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, returns the flight-offers with included checked bags only\"\n    },\n    \"refundableFare\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, returns the flight-offers with refundable fares only\"\n    },\n    \"noRestrictionFare\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, returns the flight-offers with no restriction fares only\"\n    },\n    \"noPenaltyFare\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, returns the flight-offers with no penalty fares only\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-search-extendedpricingoptions-schema.json
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
title: ExtendedPricingOptions
---
