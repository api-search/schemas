---
description: The Warning Definition
layout: schema
name: warnings
properties_list:
- description: A machine-readable warning code from the Canned Messages table, that will enable the API Consumers code to handle this type of warning
  name: code
  type: integer
- description: An warning title from the Canned Messages table with a 1:1 correspondence to the error code. This may be localized
  name: title
  type: string
- description: An easy-to-read explanation specific to this occurrence of the problem. It should give the API consumer an idea of what went wrong and how to recover from it. Like the title, this field’s value can be
  name: detail
  type: string
- description: The Warning Source Definition
  name: source
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-warnings-schema.json
slug: trip-parser-warnings
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
title: warnings
---
