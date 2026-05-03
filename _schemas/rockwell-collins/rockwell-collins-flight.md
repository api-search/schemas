---
description: Schema representing a flight record from the FlightAware AeroAPI, including identification, routing, timing, and status information.
layout: schema
name: FlightAware AeroAPI Flight
properties_list:
- description: Flight identifier (airline code + flight number, e.g., UAL123)
  name: ident
  type: string
- description: ICAO flight identifier
  name: ident_icao
  type: string
- description: IATA flight identifier
  name: ident_iata
  type: string
- description: Unique FlightAware flight ID for this specific flight instance
  name: fa_flight_id
  type: string
- description: Operator ICAO code (e.g., UAL for United Airlines)
  name: operator
  type: string
- description: Operator IATA code
  name: operator_iata
  type: string
- description: Airline flight number
  name: flight_number
  type: string
- description: Aircraft tail number / registration
  name: registration
  type: string
- description: ICAO aircraft type code (e.g., B738)
  name: aircraft_type
  type: string
- description: Departure airport information
  name: origin
  type: object
- description: Arrival airport information
  name: destination
  type: object
- description: Departure delay in seconds (negative = early)
  name: departure_delay
  type: integer
- description: Arrival delay in seconds (negative = early)
  name: arrival_delay
  type: integer
- description: Filed estimated time en route in seconds
  name: filed_ete
  type: integer
- description: Scheduled gate departure time (pushback)
  name: scheduled_out
  type: string
- description: Estimated gate departure time
  name: estimated_out
  type: string
- description: Actual gate departure time
  name: actual_out
  type: string
- description: Scheduled takeoff time
  name: scheduled_off
  type: string
- description: Estimated takeoff time
  name: estimated_off
  type: string
- description: Actual takeoff time
  name: actual_off
  type: string
- description: Scheduled landing time
  name: scheduled_on
  type: string
- description: Estimated landing time
  name: estimated_on
  type: string
- description: Actual landing time
  name: actual_on
  type: string
- description: Current flight status
  name: status
  type: string
- description: Estimated flight completion percentage
  name: progress_percent
  type: integer
- description: Filed route string
  name: route
  type: string
- description: Filed true airspeed in knots
  name: filed_airspeed
  type: integer
- description: Filed cruise altitude in hundreds of feet
  name: filed_altitude
  type: integer
- description: Whether FlightAware Foresight ML predictions are available for this flight
  name: foresight_predictions_available
  type: boolean
provider_name: Rockwell Collins
provider_slug: rockwell-collins
schema_file: json-schema/rockwell-collins-flight-schema.json
slug: rockwell-collins-flight
source_filename: rockwell-collins-flight-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/rockwell-collins/json-schema/rockwell-collins-flight-schema.json\",\n  \"title\": \"FlightAware AeroAPI Flight\",\n  \"description\": \"Schema representing a flight record from the FlightAware AeroAPI, including identification, routing, timing, and status information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ident\": {\n      \"type\": \"string\",\n      \"description\": \"Flight identifier (airline code + flight number, e.g., UAL123)\"\n    },\n    \"ident_icao\": {\n      \"type\": \"string\",\n      \"description\": \"ICAO flight identifier\"\n    },\n    \"ident_iata\": {\n      \"type\": \"string\",\n      \"description\": \"IATA flight identifier\"\n    },\n    \"fa_flight_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique FlightAware flight ID for this specific flight instance\"\n    },\n    \"operator\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Operator ICAO code (e.g., UAL for United Airlines)\"\n    },\n    \"operator_iata\": {\n      \"type\": \"string\",\n      \"description\": \"Operator IATA code\"\n    },\n    \"flight_number\": {\n      \"type\": \"string\",\n      \"description\": \"Airline flight number\"\n    },\n    \"registration\": {\n      \"type\": \"string\",\n      \"description\": \"Aircraft tail number / registration\"\n    },\n    \"aircraft_type\": {\n      \"type\": \"string\",\n      \"description\": \"ICAO aircraft type code (e.g., B738)\"\n    },\n    \"origin\": {\n      \"type\": \"object\",\n      \"description\": \"Departure airport information\",\n      \"properties\": {\n        \"code\": { \"type\": \"string\" },\n        \"code_icao\": { \"type\": \"string\" },\n        \"code_iata\": { \"type\": \"string\" },\n        \"airport_info_url\": { \"type\": \"string\", \"format\": \"uri\" }\n      }\n    },\n    \"destination\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Arrival airport information\",\n      \"properties\": {\n        \"code\": { \"type\": \"string\" },\n        \"code_icao\": { \"type\": \"string\" },\n        \"code_iata\": { \"type\": \"string\" },\n        \"airport_info_url\": { \"type\": \"string\", \"format\": \"uri\" }\n      }\n    },\n    \"departure_delay\": {\n      \"type\": \"integer\",\n      \"description\": \"Departure delay in seconds (negative = early)\"\n    },\n    \"arrival_delay\": {\n      \"type\": \"integer\",\n      \"description\": \"Arrival delay in seconds (negative = early)\"\n    },\n    \"filed_ete\": {\n      \"type\": \"integer\",\n      \"description\": \"Filed estimated time en route in seconds\"\n    },\n    \"scheduled_out\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scheduled gate departure time (pushback)\"\n    },\n    \"estimated_out\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Estimated gate departure time\"\n    },\n    \"actual_out\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Actual gate departure time\"\n    },\n    \"scheduled_off\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scheduled takeoff time\"\n    },\n    \"estimated_off\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Estimated takeoff time\"\n    },\n    \"actual_off\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Actual takeoff time\"\n    },\n    \"scheduled_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scheduled landing time\"\n    },\n    \"estimated_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Estimated landing time\"\n    },\n    \"actual_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"Actual landing time\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Scheduled\", \"Active\", \"En Route\", \"Landed\", \"Cancelled\", \"Diverted\"],\n      \"description\": \"Current flight status\"\n    },\n    \"progress_percent\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Estimated flight completion percentage\"\n    },\n    \"route\": {\n      \"type\": \"string\",\n      \"description\": \"Filed route string\"\n    },\n    \"filed_airspeed\": {\n      \"type\": \"integer\",\n      \"description\": \"Filed true airspeed in knots\"\n    },\n    \"filed_altitude\": {\n      \"type\": \"integer\",\n      \"description\": \"Filed cruise altitude in hundreds of feet\"\n    },\n    \"foresight_predictions_available\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether FlightAware Foresight ML predictions are available for this flight\"\n    }\n  },\n  \"\
  additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rockwell-collins/refs/heads/main/json-schema/rockwell-collins-flight-schema.json
tags:
- Avionics
- Aerospace
- Defense
- Aviation
- Flight Deck
title: FlightAware AeroAPI Flight
---
