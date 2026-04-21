---
description: Warning
layout: schema
name: Warning
properties_list:
- description: '[Integer] A machine-readable warning code from the Amadeus Canned Messages table, that will enable the API Consumers code to handle this type of warning'
  name: code
  type: integer
- description: '[String] A warning title from the Canned Messages table with a 1:1 correspondence to the warning code. This may be localized'
  name: title
  type: string
- description: '[String] An easy-to-read explanation specific to this occurrence of the problem. It should give the API consumer an idea of what went wrong and how to recover from it. Like the title, this field value'
  name: detail
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-booking-warning-schema.json
slug: hotel-booking-warning
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
title: Warning
---
