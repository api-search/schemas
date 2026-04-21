---
description: Some prices may vary during a stay, thus here you can see the daily price per period of the stay
layout: schema
name: HotelProduct_PriceVariation
properties_list:
- description: 'Begin date of the period Format: YYYY-MM-DD'
  name: startDate
  type: string
- description: 'End date of the period Format: YYYY-MM-DD'
  name: endDate
  type: string
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
schema_file: json-schema/hotel-search-hotelproduct-pricevariation-schema.json
slug: hotel-search-hotelproduct-pricevariation
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
title: HotelProduct_PriceVariation
---
