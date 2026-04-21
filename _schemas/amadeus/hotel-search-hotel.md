---
description: Hotel Content
layout: schema
name: Hotel
properties_list:
- description: Amadeus Property Code (8 chars)
  name: hotelId
  type: string
- description: Brand (RT...) or Merchant (AD...) (Amadeus 2 chars Code)
  name: chainCode
  type: string
- description: Brand (RT...) (Amadeus 2 chars Code). Small Properties distributed by Merchants may not have a Brand. Example - AD (Value Hotels) is the Provider/Merchant, and RT (Accor) is the Brand of the Property
  name: brandCode
  type: string
- description: Unique Property identifier of the physical hotel. One physical hotel can be represented by different Providers, each one having its own `hotelID`. This attribute allows a client application to group t
  name: dupeId
  type: string
- description: Hotel Name
  name: name
  type: string
- description: 'Warning: The IATA city code associated to the hotel (not necessary the real Hotel City)'
  name: cityCode
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotel-schema.json
slug: hotel-search-hotel
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
title: Hotel
---
