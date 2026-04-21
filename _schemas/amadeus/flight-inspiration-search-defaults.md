---
description: the query parameters for which default values were used are returned here
layout: schema
name: Defaults
properties_list:
- description: the date, or range of dates, on which the flight will depart from the origin. Dates are specified in the [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-DD format, e.g. 2017-12-25. Ranges a
  name: departureDate
  type: string
- description: if this parameter is set to true, only one-way flights are considered. If this parameter is not set or set to false, only round-trip flights are considered
  name: oneWay
  type: boolean
- description: exact duration or range of durations of the travel, in days. This parameter must not be set if oneWay is true. Ranges are specified with a comma and are inclusive, e.g. 2,8
  name: duration
  type: string
- description: if this parameter is set to true, only flights going from the origin to the destination with no stop in-between are considered
  name: nonStop
  type: boolean
- description: view the flight destinations by COUNTRY, DATE, DESTINATION, DURATION, or WEEK. View by COUNTRY to get the cheapest flight dates for every country in the given range. View by DATE to get the cheapest f
  name: viewBy
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-inspiration-search-defaults-schema.json
slug: flight-inspiration-search-defaults
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
title: Defaults
---
