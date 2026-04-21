---
description: ticketing agreement
layout: schema
name: TicketingAgreement
properties_list:
- description: ''
  name: option
  type: object
- description: Delay before applying automatic process if no issuance in days
  name: delay
  type: string
- description: Exact date to apply automatic process if no issuance. YYYY-MM-DD format, e.g. 2019-06-07
  name: dateTime
  type: string
- description: Ids of the impacted segments
  name: segmentIds
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-create-orders-ticketingagreement-schema.json
slug: flight-create-orders-ticketingagreement
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
title: TicketingAgreement
---
