---
description: ArrivalFlightDetails schema
layout: schema
name: ArrivalFlightDetails
properties_list:
- description: Carrier code
  name: carrierCode
  type: string
- description: Flight segment number
  name: number
  type: string
- description: Departure or arrival information
  name: departure
  type: object
- description: Departure or arrival information
  name: arrival
  type: object
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-arrival-flight-details-schema.json
slug: hotel-booking-arrival-flight-details
source_filename: hotel-booking-arrival-flight-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-arrival-flight-details-schema.json\",\n  \"title\": \"ArrivalFlightDetails\",\n  \"description\": \"ArrivalFlightDetails schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"carrierCode\": {\n      \"type\": \"string\",\n      \"description\": \"Carrier code\",\n      \"example\": \"LH\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Flight segment number\",\n      \"example\": \"1050\"\n    },\n    \"departure\": {\n      \"type\": \"object\",\n      \"description\": \"Departure or arrival information\",\n      \"title\": \"FlightSegment_Departure\",\n      \"required\": [\n        \"iataCode\"\n      ],\n      \"properties\": {\n        \"iataCode\": {\n          \"description\": \"IATA Airport code\",\n          \"type\": \"string\",\n\
  \          \"example\": \"JFK\"\n        }\n      }\n    },\n    \"arrival\": {\n      \"type\": \"object\",\n      \"description\": \"Departure or arrival information\",\n      \"title\": \"FlightSegment_Arrival\",\n      \"properties\": {\n        \"iataCode\": {\n          \"description\": \"IATA Airport code\",\n          \"type\": \"string\",\n          \"example\": \"JFK\"\n        },\n        \"terminal\": {\n          \"description\": \"Terminal name / number\",\n          \"type\": \"string\",\n          \"example\": \"T2\"\n        },\n        \"at\": {\n          \"description\": \"Local date and time at the arrival of the flight with the following format \\\"YYYY-MM-DD'T'HH:mm:ss\\\" (for example 2017-02-10T20:40:00 if the flight arrive 20h40 local time)\",\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"example\": \"2017-10-23T20:00:00+02:00\"\n        }\n      },\n      \"required\": [\n        \"iataCode\",\n        \"terminal\",\n   \
  \     \"at\"\n      ]\n    }\n  },\n  \"required\": [\n    \"carrierCode\",\n    \"number\",\n    \"departure\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-arrival-flight-details-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: ArrivalFlightDetails
---
