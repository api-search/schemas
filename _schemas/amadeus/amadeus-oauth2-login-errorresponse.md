---
description: Error responses are sent when an error (e.g. unauthorized, bad request, ...) occurred.
layout: schema
name: ErrorResponse
properties_list:
- description: Name is the error name.
  name: error
  type: string
- description: A small description about the error
  name: error_description
  type: string
- description: Debug contains debug information.
  name: code
  type: integer
- description: Debug contains debug information. This is usually not available and has to be enabled.
  name: title
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/amadeus-oauth2-login-errorresponse-schema.json
slug: amadeus-oauth2-login-errorresponse
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
title: ErrorResponse
---
