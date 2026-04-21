---
description: price metric
layout: schema
name: itinerary-price-metric
properties_list:
- description: ressource type - always price-metrics
  name: type
  type: string
- description: Description of a particular point or place in physical space
  name: origin
  type: object
- description: Description of a particular point or place in physical space
  name: destination
  type: object
- description: The date on which the traveler will depart from the origin to go to the destination. Dates are specified in the[ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-DD format.
  name: departureDate
  type: string
- description: transportation type
  name: transportType
  type: string
- description: currency of the prices. Currency is specified in the [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) format, e.g. EUR for Euro
  name: currencyCode
  type: string
- description: true for a one way trip, false for a round trip
  name: oneWay
  type: boolean
- description: ''
  name: priceMetrics
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-price-analysis-itinerary-price-metric-schema.json
slug: flight-price-analysis-itinerary-price-metric
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
title: itinerary-price-metric
---
