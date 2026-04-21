---
description: input parameter to price flight offers element
layout: schema
name: FlightOfferPricingIn
properties_list:
- description: the resource name
  name: type
  type: string
- description: list of flight offer to price
  name: flightOffers
  type: array
- description: payment information for retrieve eventual credit card fees
  name: payments
  type: array
- description: list of travelers
  name: travelers
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-price-flightofferpricingin-schema.json
slug: flight-offers-price-flightofferpricingin
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
title: FlightOfferPricingIn
---
