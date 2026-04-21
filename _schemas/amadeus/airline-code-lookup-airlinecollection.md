---
description: A collection response containing an array of airline resources and associated metadata.
layout: schema
name: AirlineCollection
properties_list:
- description: ''
  name: meta
  type: object
- description: Array of airline resources matching the query.
  name: data
  type: array
- description: Non-blocking issues encountered during the request processing.
  name: warnings
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airline-code-lookup-airlinecollection-schema.json
slug: airline-code-lookup-airlinecollection
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
title: AirlineCollection
---
