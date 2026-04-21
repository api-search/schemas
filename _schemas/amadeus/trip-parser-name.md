---
description: Description of the name of a physical person
layout: schema
name: name
properties_list:
- description: First name.
  name: firstName
  type: string
- description: Last name.
  name: lastName
  type: string
- description: Contains all the suffixes and prefixes that can be appended to a name - Mr, Miss, Pr. - E.g. " Mr".
  name: title
  type: string
- description: Middle name(s), for example "Lee" in "John Lee Smith".
  name: middleName
  type: string
- description: Name prefix (e.g. Doctor)
  name: prefix
  type: string
- description: Name suffix (e.g. Junior, III, etc).
  name: suffix
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-name-schema.json
slug: trip-parser-name
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
title: name
---
