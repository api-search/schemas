---
description: ''
layout: schema
name: PassengerCharacteristics
properties_list:
- description: Passenger type codes e.g. CHD , ADT. CHD is for child and ADT for Adult.
  name: passengerTypeCode
  type: string
- description: Age of the Passenger (Mandatory if typeCode= “CHD”)
  name: age
  type: integer
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-passengercharacteristics-schema.json
slug: transfer-booking-passengercharacteristics
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
title: PassengerCharacteristics
---
