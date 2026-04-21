---
description: price information
layout: schema
name: HotelProduct_HotelPrice
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
  name: taxes
  type: array
- description: ''
  name: markups
  type: array
- description: ''
  name: variations
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotelproduct-hotelprice-schema.json
slug: hotel-search-hotelproduct-hotelprice
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
title: HotelProduct_HotelPrice
---
