---
description: Car Product
layout: schema
name: carData
properties_list:
- description: Confirmation number
  name: confirmationNumber
  type: string
- description: car provider information(Car rental compay name)
  name: serviceProviderName
  type: string
- description: ''
  name: associatedEquipments
  type: array
- description: ''
  name: pickup
  type: object
- description: ''
  name: dropoff
  type: object
- description: ''
  name: driver
  type: object
- description: ''
  name: vehicle
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-cardata-schema.json
slug: trip-parser-cardata
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
title: carData
---
