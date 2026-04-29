---
description: ''
layout: schema
name: DatedFlight
properties_list:
- description: the resource name
  name: type
  type: string
- description: the scheduled departure date
  name: scheduledDepartureDate
  type: string
- description: ''
  name: flightDesignator
  type: object
- description: the flight points of the flight. At least one departure, one arrival
  name: flightPoints
  type: array
- description: 'the list of segments of the datedFlight - definition of segment: the commercial unit corresponding to the passenger journey traveling between two points with the same flight (same flight designator)'
  name: segments
  type: array
- description: 'the list of legs of the datedFlight. - definition of leg: operation of the aircraft between a departure station and the next arrival station (between take off and landing)'
  name: legs
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/on-demand-flight-status-datedflight-schema.json
slug: on-demand-flight-status-datedflight
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DatedFlight\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"the resource name\"\n    },\n    \"scheduledDepartureDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"the scheduled departure date\"\n    },\n    \"flightDesignator\": {\n      \"$ref\": \"#/definitions/FlightDesignator\"\n    },\n    \"flightPoints\": {\n      \"type\": \"array\",\n      \"description\": \"the flight points of the flight.\\nAt least one departure, one arrival\\n\",\n      \"items\": {\n        \"$ref\": \"#/definitions/FlightPoint\"\n      }\n    },\n    \"segments\": {\n      \"type\": \"array\",\n      \"description\": \"the list of segments of the datedFlight\\n- definition of segment: the commercial unit corresponding to the passenger journey traveling between two points with the same flight (same flight\
  \ designator)\\n\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Segment\"\n      }\n    },\n    \"legs\": {\n      \"type\": \"array\",\n      \"description\": \"the list of legs of the datedFlight.\\n- definition of leg: operation of the aircraft between a departure station and the next arrival station (between take off and landing)\\n\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Leg\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/on-demand-flight-status-datedflight-schema.json
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
title: DatedFlight
---
