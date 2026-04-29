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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-extended-pricing-options-schema.json
slug: flight-offers-search-extended-pricing-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-extended-pricing-options-schema.json\",\n  \"title\": \"ExtendedPricingOptions\",\n  \"description\": \"fare filter options\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"includedCheckedBagsOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, returns the flight-offers with included checked bags only\",\n      \"example\": true\n    },\n    \"refundableFare\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, returns the flight-offers with refundable fares only\",\n      \"example\": true\n    },\n    \"noRestrictionFare\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, returns the flight-offers with no restriction fares only\",\n      \"example\": true\n    },\n    \"noPenaltyFare\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"If true, returns the flight-offers with no penalty fares only\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-extended-pricing-options-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: ExtendedPricingOptions
---
