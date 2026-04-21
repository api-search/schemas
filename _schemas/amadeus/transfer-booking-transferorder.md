---
description: ''
layout: schema
name: TransferOrder
properties_list:
- description: the resource name
  name: type
  type: string
- description: transfer order identifier
  name: id
  type: string
- description: reference of the Trip e.g. YNK4JQ
  name: reference
  type: string
- description: transfer reservations, included in the order
  name: transfers
  type: array
- description: passengers, related to the Transfer Order
  name: passengers
  type: array
- description: ''
  name: agency
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-transferorder-schema.json
slug: transfer-booking-transferorder
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
title: TransferOrder
---
