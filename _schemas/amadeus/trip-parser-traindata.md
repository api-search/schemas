---
description: Train Product
layout: schema
name: trainData
properties_list:
- description: Confirmation number
  name: confirmNbr
  type: string
- description: Provider name
  name: serviceProviderName
  type: string
- description: Booking class
  name: bookingClass
  type: string
- description: ''
  name: departure
  type: object
- description: Date in ISO 8601 (http://www.w3.org/TR/NOTE-datetime), YYYY-MM-DDTHH:MM:SSZ.
  name: departureDateTime
  type: string
- description: Date in ISO 8601 (http://www.w3.org/TR/NOTE-datetime), YYYY-MM-DDTHH:MM:SSZ.
  name: arrivalDateTime
  type: string
- description: ''
  name: arrival
  type: object
- description: Duration in ISO 8601 / RFC 3339 (https://www.ietf.org/rfc/rfc3339.txt), P[n]Y[n]M[n]DT[n]H[n]M[n]S.
  name: duration
  type: string
- description: ''
  name: departureTrack
  type: string
- description: ''
  name: arrivalTrack
  type: string
- description: ''
  name: seats
  type: array
- description: ''
  name: vehicle
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-traindata-schema.json
slug: trip-parser-traindata
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
title: trainData
---
