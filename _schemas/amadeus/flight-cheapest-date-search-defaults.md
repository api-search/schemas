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
- description: view the flight dates by DATE, DURATION, or WEEK. View by DATE to get the cheapest flight dates for every departure date in the given range. View by DURATION to get the cheapest flight dates for every
  name: viewBy
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-cheapest-date-search-defaults-schema.json
slug: flight-cheapest-date-search-defaults
source_filename: flight-cheapest-date-search-defaults-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Defaults\",\n  \"description\": \"the query parameters for which default values were used are returned here\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"departureDate\": {\n      \"type\": \"string\",\n      \"description\": \"the date, or range of dates, on which the flight will depart from the origin. Dates are specified in the [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-DD format, e.g. 2017-12-25. Ranges are specified with a comma and are inclusive\"\n    },\n    \"oneWay\": {\n      \"type\": \"boolean\",\n      \"description\": \"if this parameter is set to true, only one-way flights are considered. If this parameter is not set or set to false, only round-trip flights are considered\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"exact duration or range of durations of the travel, in days. This parameter must not be set if oneWay\
  \ is true. Ranges are specified with a comma and are inclusive, e.g. 2,8\"\n    },\n    \"nonStop\": {\n      \"type\": \"boolean\",\n      \"description\": \"if this parameter is set to true, only flights going from the origin to the destination with no stop in-between are considered\"\n    },\n    \"viewBy\": {\n      \"type\": \"string\",\n      \"description\": \"view the flight dates by DATE, DURATION, or WEEK. View by DATE to get the cheapest flight dates for every departure date in the given range. View by DURATION to get the cheapest flight dates for every departure date and for every duration in the given ranges. View by WEEK to get the cheapest flight date for every week in the given range of departure dates\",\n      \"enum\": [\n        \"DATE\",\n        \"DURATION\",\n        \"WEEK\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-cheapest-date-search-defaults-schema.json
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
