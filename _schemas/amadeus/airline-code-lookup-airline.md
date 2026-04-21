---
description: An airline resource containing identifying codes and names for a single airline carrier.
layout: schema
name: Airline
properties_list:
- description: Resource type identifier.
  name: type
  type: string
- description: Two-letter IATA airline designator code.
  name: iataCode
  type: string
- description: Three-letter ICAO airline designator code.
  name: icaoCode
  type: string
- description: The official business name of the airline.
  name: businessName
  type: string
- description: The commonly used abbreviated name of the airline.
  name: commonName
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airline-code-lookup-airline-schema.json
slug: airline-code-lookup-airline
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
title: Airline
---
