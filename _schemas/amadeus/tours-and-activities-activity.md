---
description: Activity description
layout: schema
name: Activity
properties_list:
- description: the ressource name
  name: type
  type: string
- description: unique id of the ressource
  name: id
  type: string
- description: ''
  name: self
  type: object
- description: activity name
  name: name
  type: string
- description: short description of the activity
  name: shortDescription
  type: string
- description: full description of the activity
  name: description
  type: string
- description: ''
  name: geoCode
  type: object
- description: rating of the activity
  name: rating
  type: string
- description: ''
  name: price
  type: object
- description: link to picture related to the activity
  name: pictures
  type: array
- description: url to book the activity
  name: bookingLink
  type: string
- description: Minimum recommended duration for the activity
  name: minimumDuration
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/tours-and-activities-activity-schema.json
slug: tours-and-activities-activity
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
title: Activity
---
