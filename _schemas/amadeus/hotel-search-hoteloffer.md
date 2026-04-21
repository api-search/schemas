---
description: Hotel Offer
layout: schema
name: HotelOffer
properties_list:
- description: ''
  name: type
  type: object
- description: Unique identifier of this offer. Might be valid for a temporary period only.
  name: id
  type: string
- description: check-in date of the stay (hotel local date). Format YYYY-MM-DD The lowest accepted value is today date (no dates in the past).
  name: checkInDate
  type: string
- description: check-out date of the stay (hotel local date). Format YYYY-MM-DD The lowest accepted value is `checkInDate`+1.
  name: checkOutDate
  type: string
- description: number of rooms (1-9)
  name: roomQuantity
  type: string
- description: Special Rate - Provider Response Code (3 chars) Examples * RAC - Rack * BAR - Best Available Rate * PRO - Promotional * COR - Corporate * GOV - Government (qualified) * AAA - AAA (qualified) * BNB - B
  name: rateCode
  type: string
- description: ''
  name: rateFamilyEstimated
  type: object
- description: 'Special Rate Category Examples: ASSOCIATION FAMILY_PLAN'
  name: category
  type: string
- description: ''
  name: description
  type: object
- description: ''
  name: commission
  type: object
- description: ''
  name: boardType
  type: object
- description: ''
  name: room
  type: object
- description: ''
  name: guests
  type: object
- description: ''
  name: price
  type: object
- description: ''
  name: policies
  type: object
- description: A self link to the object. Use this to refresh the Offer price
  name: self
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hoteloffer-schema.json
slug: hotel-search-hoteloffer
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
title: HotelOffer
---
