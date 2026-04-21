---
description: Definition of PNR travelers. Fields gender, nationality, placeOfBirth, countryOfResidence are only populated for passengerDelivery resources.
layout: schema
name: stakeholder
properties_list:
- description: item identifier
  name: id
  type: string
- description: Nationality of the Stakeholder
  name: nationality
  type: string
- description: '3-characters code defining the passenger type - possible values: ADT, CHD, INS, INF, UNA'
  name: passangerTypeCode
  type: string
- description: The individual's date of birth.
  name: dateOfBirth
  type: string
- description: Current age of the individual.
  name: age
  type: integer
- description: ''
  name: name
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-stakeholder-schema.json
slug: trip-parser-stakeholder
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
title: stakeholder
---
