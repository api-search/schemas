---
description: ''
layout: schema
name: ErrorSource
properties_list:
- description: The key of the URI path or query parameter that caused the error
  name: parameter
  type: string
- description: A JSON Pointer [RFC6901] to the associated entity in the request body that caused this error
  name: pointer
  type: string
- description: A sample input to guide the user when resolving this issue
  name: example
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-ratings-errorsource-schema.json
slug: hotel-ratings-errorsource
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
title: ErrorSource
---
