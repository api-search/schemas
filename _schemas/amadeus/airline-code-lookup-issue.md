---
description: A non-blocking warning or issue encountered during request processing.
layout: schema
name: Issue
properties_list:
- description: HTTP status code associated with the issue.
  name: status
  type: integer
- description: Application-specific error code.
  name: code
  type: integer
- description: Short description of the issue.
  name: title
  type: string
- description: Detailed explanation of the issue.
  name: detail
  type: string
- description: ''
  name: source
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airline-code-lookup-issue-schema.json
slug: airline-code-lookup-issue
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
