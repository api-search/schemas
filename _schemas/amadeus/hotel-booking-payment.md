---
description: form of payment (mandatory in case of `acceptedPayments`/`methods`)
layout: schema
name: Payment
properties_list:
- description: ''
  name: id
  type: integer
- description: 'The Payment Methods: * creditCard (CC) - Payment Cards in `creditCards` are accepted'
  name: method
  type: string
- description: payment card details (mandatory in case of `method` creditCard)
  name: card
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-booking-payment-schema.json
slug: hotel-booking-payment
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
title: Payment
---
