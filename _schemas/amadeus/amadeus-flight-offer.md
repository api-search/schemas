---
description: A flight offer returned by the Amadeus Flight Offers Search API, representing a purchasable combination of flight segments with pricing for one or more travelers.
layout: schema
name: Amadeus Flight Offer
properties_list:
- description: Resource type identifier for a flight offer.
  name: type
  type: string
- description: Unique identifier for the flight offer within the search results.
  name: id
  type: string
- description: Source of the flight offer data.
  name: source
  type: string
- description: Whether the offer requires immediate ticketing upon booking.
  name: instantTicketingRequired
  type: boolean
- description: Whether the offer contains segments with different booking classes.
  name: nonHomogeneous
  type: boolean
- description: Whether the offer is for a one-way trip.
  name: oneWay
  type: boolean
- description: Last date by which the flight must be ticketed, in ISO 8601 YYYY-MM-DD format.
  name: lastTicketingDate
  type: string
- description: Last date and time by which the flight must be ticketed, in ISO 8601 format.
  name: lastTicketingDateTime
  type: string
- description: Number of seats remaining available for booking on this offer.
  name: numberOfBookableSeats
  type: integer
- description: Array of itineraries composing the trip, each containing one or more flight segments.
  name: itineraries
  type: array
- description: Total price of the flight offer including all travelers.
  name: price
  type: object
- description: Pricing options and fare rules applicable to this offer.
  name: pricingOptions
  type: object
- description: IATA codes of the airlines validating and issuing the tickets.
  name: validatingAirlineCodes
  type: array
- description: Individual pricing breakdown for each traveler on the booking.
  name: travelerPricings
  type: array
- description: Reference dictionaries for codes used in the offer including carriers, aircraft, currencies, and locations.
  name: dictionaries
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/amadeus-flight-offer-schema.json
slug: amadeus-flight-offer
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
title: Amadeus Flight Offer
---
