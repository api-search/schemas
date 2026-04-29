---
description: ''
layout: schema
name: DateTimeType
properties_list:
- description: Dates are specified in the [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-DD format, e.g. 2018-12-25
  name: date
  type: string
- description: Local time. hh:mm:ss format, e.g 10:30:00
  name: time
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-availibilities-search-datetimetype-schema.json
slug: flight-availibilities-search-datetimetype
source_filename: flight-availibilities-search-datetimetype-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DateTimeType\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Dates are specified in the [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-DD format, e.g. 2018-12-25\"\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"description\": \"Local time. hh:mm:ss format, e.g 10:30:00\"\n    }\n  },\n  \"required\": [\n    \"date\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-availibilities-search-datetimetype-schema.json
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
title: DateTimeType
---
