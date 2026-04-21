---
description: A hotel offer returned by the Amadeus Hotel Search API, representing a bookable room at a specific hotel with pricing, room details, and guest information.
layout: schema
name: Amadeus Hotel Offer
properties_list:
- description: Resource type identifier for hotel offers.
  name: type
  type: string
- description: Hotel property information.
  name: hotel
  type: object
- description: Whether the hotel has offers available for the requested dates.
  name: available
  type: boolean
- description: Array of bookable offers for the hotel.
  name: offers
  type: array
- description: Self link to this hotel offer resource.
  name: self
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/amadeus-hotel-offer-schema.json
slug: amadeus-hotel-offer
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
title: Amadeus Hotel Offer
---
