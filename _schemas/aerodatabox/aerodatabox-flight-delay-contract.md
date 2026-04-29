---
description: Delay statistics for a flight movement
layout: schema
name: FlightDelayContract
properties_list:
- description: ICAO code of the airport at which statistics is observed
  name: airportIcao
  type: string
- description: ''
  name: class
  type: object
- description: Hour on which flight is scheduled (represented in UTC). If provided, it separates the statistics for the same flight departing/arriving at different time of day on different days within the observed p
  name: scheduledHourUtc
  type: integer
- description: 'Median historic delay of the flight (format: [-]hh:mm:ss). Value can be negative (therefore, means early occurence).'
  name: medianDelay
  type: string
- description: Distribution of historic delays of the flight in percentiles from 5 percentile to 95 percentile in steps of 5 percentile, allowing for a more detailed analysis of delay patterns beyond simple averages
  name: delayPercentiles
  type: array
- description: The number of flight movements taken into account to calculate this statistics.
  name: numConsideredFlights
  type: integer
- description: Brackets containing information more detailed information about how many flights were delayed/early per specific delay range brackets (e.g. late from 15 to 30 minutes, from 30 to 60, etc.)
  name: numFlightsDelayedBrackets
  type: array
- description: The beginning of the time range within which flght delay information is calculated (represented in UTC time)
  name: fromUtc
  type: string
- description: The end of the time range within which flght delay information is calculated (represented in UTC time)
  name: toUtc
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-flight-delay-contract-schema.json
slug: aerodatabox-flight-delay-contract
source_filename: aerodatabox-flight-delay-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-delay-contract-schema.json\",\n  \"title\": \"FlightDelayContract\",\n  \"description\": \"Delay statistics for a flight movement\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"airportIcao\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"ICAO code of the airport at which statistics is observed\"\n    },\n    \"class\": {\n      \"$ref\": \"#/components/schemas/StatisticClass\"\n    },\n    \"scheduledHourUtc\": {\n      \"type\": \"integer\",\n      \"description\": \"Hour on which flight is scheduled (represented in UTC).\\r\\n\\r\\nIf provided, it separates the statistics for the same flight departing/arriving at different time of day\\r\\non different days within the observed period.\",\n      \"format\": \"int32\",\n      \"nullable\": true\n\
  \    },\n    \"medianDelay\": {\n      \"type\": \"string\",\n      \"description\": \"Median historic delay of the flight (format: [-]hh:mm:ss).\\r\\nValue can be negative (therefore, means early occurence).\",\n      \"format\": \"date-span\"\n    },\n    \"delayPercentiles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PercentileBracketContract\"\n      },\n      \"description\": \"Distribution of historic delays of the flight in percentiles from 5 percentile to 95 percentile in steps of 5 percentile, \\r\\nallowing for a more detailed analysis of delay patterns beyond simple averages or medians.\"\n    },\n    \"numConsideredFlights\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of flight movements taken into account to calculate this\\r\\nstatistics.\",\n      \"format\": \"int32\"\n    },\n    \"numFlightsDelayedBrackets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DelayBracketContract\"\
  \n      },\n      \"description\": \"Brackets containing information more detailed information about\\r\\nhow many flights were delayed/early per specific delay range brackets\\r\\n(e.g. late from 15 to 30 minutes, from 30 to 60, etc.)\"\n    },\n    \"fromUtc\": {\n      \"type\": \"string\",\n      \"description\": \"The beginning of the time range within which flght delay information is calculated (represented in UTC time)\",\n      \"format\": \"date-time\"\n    },\n    \"toUtc\": {\n      \"type\": \"string\",\n      \"description\": \"The end of the time range within which flght delay information is calculated (represented in UTC time)\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"airportIcao\",\n    \"class\",\n    \"delayPercentiles\",\n    \"fromUtc\",\n    \"medianDelay\",\n    \"numConsideredFlights\",\n    \"numFlightsDelayedBrackets\",\n    \"toUtc\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-delay-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FlightDelayContract
---
