---
description: ''
layout: schema
name: OtherServices
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: price
  type: object
- description: Specify if the service is bookable by traveler or for all travelers
  name: bookableByTraveler
  type: boolean
- description: Specify if the service is bookable by itinerary or for all itineraries
  name: bookableByItinerary
  type: boolean
- description: Id of the segment concerned by the service
  name: segmentIds
  type: array
- description: Id of the traveler concerned by the service
  name: travelerIds
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-price-otherservices-schema.json
slug: flight-offers-price-otherservices
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
title: OtherServices
---
