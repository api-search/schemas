---
description: Electronic ticket for a passenger on a BlaBlaCar Bus trip
layout: schema
name: Ticket
properties_list:
- description: Unique ticket identifier
  name: ticket_id
  type: string
- description: Associated booking identifier
  name: booking_id
  type: string
- description: Full name of the ticket holder
  name: passenger_name
  type: string
- description: Departure date and time
  name: departure_datetime
  type: string
- description: Departure station name
  name: from_station
  type: string
- description: Arrival station name
  name: to_station
  type: string
- description: Assigned seat number
  name: seat_number
  type: string
- description: Current ticket status
  name: status
  type: string
- description: Base64-encoded QR code image
  name: qr_code
  type: string
provider_name: BlaBlaCar Bus API
provider_slug: blablacar-bus-api
schema_file: json-schema/blablacar-bus-api-ticket-schema.json
slug: blablacar-bus-api-ticket
source_filename: blablacar-bus-api-ticket-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/json-schema/blablacar-bus-api-ticket-schema.json\",\n  \"title\": \"Ticket\",\n  \"description\": \"Electronic ticket for a passenger on a BlaBlaCar Bus trip\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ticket_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ticket identifier\",\n      \"example\": \"ticket-500123\"\n    },\n    \"booking_id\": {\n      \"type\": \"string\",\n      \"description\": \"Associated booking identifier\",\n      \"example\": \"booking-500123\"\n    },\n    \"passenger_name\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the ticket holder\",\n      \"example\": \"Jane Smith\"\n    },\n    \"departure_datetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Departure date and time\",\n\
  \      \"example\": \"2025-06-15T07:00:00Z\"\n    },\n    \"from_station\": {\n      \"type\": \"string\",\n      \"description\": \"Departure station name\",\n      \"example\": \"Paris Bercy\"\n    },\n    \"to_station\": {\n      \"type\": \"string\",\n      \"description\": \"Arrival station name\",\n      \"example\": \"Lyon Perrache\"\n    },\n    \"seat_number\": {\n      \"type\": \"string\",\n      \"description\": \"Assigned seat number\",\n      \"example\": \"14A\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current ticket status\",\n      \"enum\": [\n        \"valid\",\n        \"used\",\n        \"cancelled\"\n      ],\n      \"example\": \"valid\"\n    },\n    \"qr_code\": {\n      \"type\": \"string\",\n      \"description\": \"Base64-encoded QR code image\",\n      \"example\": \"data:image/png;base64,abc123\"\n    }\n  },\n  \"required\": [\n    \"ticket_id\",\n    \"booking_id\",\n    \"passenger_name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/json-schema/blablacar-bus-api-ticket-schema.json
tags:
- Booking
- Buses
- Coach
- Europe
- Mobility
- Ticketing
- Transportation
- Travel
title: Ticket
---
