---
description: DateTimeRange schema
layout: schema
name: DateTimeRange
properties_list: []
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-date-time-range-schema.json
slug: flight-offers-search-date-time-range
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-date-time-range-schema.json\",\n  \"title\": \"DateTimeRange\",\n  \"description\": \"DateTimeRange schema\",\n  \"required\": [\n    \"date\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/DateTimeType\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"dateWindow\": {\n          \"description\": \"Either 1, 2 or 3 extra days around the local date (IxD for +/- x days - Ex: I3D), Either 1 to 3 days after the local date (PxD for +x days - Ex: P3D), or 1 to 3 days before the local date (MxD for -x days - Ex: M3D)\\n\\nCan not be combined with \\\"originRadius\\\" or \\\"destinationRadius\\\".\\n\",\n          \"type\": \"string\",\n          \"example\": \"I3D\",\n          \"pattern\": \"^[MPI][1-3]D\"\n        },\n        \"timeWindow\"\
  : {\n          \"description\": \"1 to 12 hours around (both +and -) the local time. Possibly limited by the number of extra days when specified, i.e.  in some situations, it may not be used to exceed the maximum date range. [1-12]H format, e.g. 6H\\n\\nCan not be combined with \\\"originRadius\\\" or \\\"destinationRadius\\\".\\n\",\n          \"type\": \"string\",\n          \"example\": \"2H\",\n          \"pattern\": \"^([1-9]|10|11|12)H\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-date-time-range-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: DateTimeRange
---
