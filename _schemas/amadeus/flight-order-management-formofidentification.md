---
description: alternative means of identifying stakeholders for eTicket.
layout: schema
name: FormOfIdentification
properties_list:
- description: Type of identification
  name: identificationType
  type: string
- description: providing the airline / carrier code
  name: carrierCode
  type: string
- description: identification number relative to the type of identification either ticket number, booking number, passport number, identity card number, drivers licence number, other ID
  name: number
  type: string
- description: Ids of the concerned travelers
  name: travelerIds
  type: array
- description: Id of the concerned flightOffers
  name: flightOfferIds
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-order-management-formofidentification-schema.json
slug: flight-order-management-formofidentification
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
title: FormOfIdentification
---
