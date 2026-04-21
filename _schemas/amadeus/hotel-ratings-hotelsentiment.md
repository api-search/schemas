---
description: ''
layout: schema
name: HotelSentiment
properties_list:
- description: Amadeus Hotel Ids are found in the Hotel Search response (parameter name is 'hotelId')
  name: hotelId
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: overallRating
  type: object
- description: ''
  name: numberOfRatings
  type: integer
- description: ''
  name: numberOfReviews
  type: integer
- description: Dictionary containing scores for all the available categories. If a property does not have any category this object will not be present in the response.
  name: sentiments
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-ratings-hotelsentiment-schema.json
slug: hotel-ratings-hotelsentiment
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
title: HotelSentiment
---
