---
description: information about provider
layout: schema
name: ServiceProvider
properties_list:
- description: provider code
  name: code
  type: string
- description: provider name
  name: name
  type: string
- description: URL to provider logo
  name: logoUrl
  type: string
- description: URL to provider's terms and conditions page
  name: termsUrl
  type: string
- description: indicates if sub-provider is preferred for the travel-seller
  name: isPreferred
  type: boolean
- description: ''
  name: contacts
  type: object
- description: list of provider settings
  name: settings
  type: array
- description: Information about the Customer stakeholder participating to the described sales summary.
  name: businessIdentification
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-serviceprovider-schema.json
slug: transfer-booking-serviceprovider
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
title: ServiceProvider
---
