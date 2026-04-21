---
description: Price valuation information
layout: schema
name: Price
properties_list:
- description: currency Code apply to all elements of the price
  name: currency
  type: string
- description: sellingTotal = Total + margins + markup + totalFees - discounts
  name: sellingTotal
  type: string
- description: total = base + totalTaxes
  name: total
  type: string
- description: ''
  name: base
  type: string
- description: ''
  name: markups
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-price-schema.json
slug: hotel-search-price
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
title: Price
---
