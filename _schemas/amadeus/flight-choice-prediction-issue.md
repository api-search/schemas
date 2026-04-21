---
description: ''
layout: schema
name: Issue
properties_list:
- description: the HTTP status code applicable to this error
  name: status
  type: integer
- description: an application-specific error code
  name: code
  type: integer
- description: a short summary of the error
  name: title
  type: string
- description: explanation of the error
  name: detail
  type: string
- description: an object containing references to the source of the error
  name: source
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-choice-prediction-issue-schema.json
slug: flight-choice-prediction-issue
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
title: Issue
---
