---
description: 'IATA Tax definition: An impost for raising revenue for the general treasury and which will be used for general public purposes.'
layout: schema
name: Tax
properties_list:
- description: Defines amount with decimal separator.
  name: amount
  type: string
- description: 'Defines a monetary unit. It is a three alpha code (iata code). Example: EUR for Euros, USD for US dollar, etc.'
  name: currency
  type: string
- description: International Standards Organization (ISO) Tax code.It is a two-letter country code.
  name: code
  type: string
- description: In the case of a tax on TST value, the percentage of the tax will be indicated in this field.
  name: percentage
  type: string
- description: Indicates if tax is included or not
  name: included
  type: boolean
- description: Example - "Governement tax"
  name: description
  type: string
- description: Specifies if the tax applies per stay or per night - PER_STAY - PER_NIGHT
  name: pricingFrequency
  type: string
- description: Specifies if the tax applies per occupant or per room - PER_OCCUPANT - PER_PRODUCT
  name: pricingMode
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-tax-schema.json
slug: hotel-search-tax
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
title: Tax
---
