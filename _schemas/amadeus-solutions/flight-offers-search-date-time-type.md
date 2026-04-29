---
description: DateTimeType schema
layout: schema
name: DateTimeType
properties_list:
- description: Dates are specified in the [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-DD format, e.g. 2018-12-25
  name: date
  type: string
- description: Local time. hh:mm:ss format, e.g 10:30:00
  name: time
  type: string
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-date-time-type-schema.json
slug: flight-offers-search-date-time-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-date-time-type-schema.json\",\n  \"title\": \"DateTimeType\",\n  \"description\": \"DateTimeType schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"description\": \"Dates are specified in the [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-DD format, e.g. 2018-12-25\",\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2018-09-22\"\n    },\n    \"time\": {\n      \"description\": \"Local time. hh:mm:ss format, e.g 10:30:00\",\n      \"type\": \"string\",\n      \"example\": \"10:30:00\"\n    }\n  },\n  \"required\": [\n    \"date\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-date-time-type-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: DateTimeType
---
