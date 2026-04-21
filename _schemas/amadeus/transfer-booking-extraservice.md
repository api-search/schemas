---
description: ''
layout: schema
name: ExtraService
properties_list:
- description: extra service code, which can take following values code | name | - DSL | Driver language specified EWT | Extra waiting time MAG | Meet & Greet FLM | Flight monitoring NWS | Newspaper CAI | Cancellati
  name: code
  type: string
- description: extra service identifier
  name: itemId
  type: string
- description: extra service description
  name: description
  type: string
- description: extra service time metric type
  name: metricType
  type: string
- description: extra service metric value
  name: metricValue
  type: string
- description: ''
  name: quotation
  type: object
- description: ''
  name: converted
  type: object
- description: true if extra service is available for booking
  name: isBookable
  type: boolean
- description: true if tax included in extra service price
  name: taxIncluded
  type: boolean
- description: true if extra service price is included in total transfer amount
  name: includedInTotal
  type: boolean
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-extraservice-schema.json
slug: transfer-booking-extraservice
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
title: ExtraService
---
