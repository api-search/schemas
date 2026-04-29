---
description: An Hotel Order is one or several hotel bookings done for a set of guest.
layout: schema
name: HotelOrder
properties_list:
- description: Array of hotel-bookings
  name: hotelBookings
  type: array
- description: Reference and origin of the hotel order record
  name: associatedRecords
  type: array
- description: Self URL for retrieving the Hotel Order
  name: self
  type: string
- description: Resource name - Is set to "hotel-order"
  name: type
  type: string
- description: ''
  name: guests
  type: object
- description: Id of the hotelorder. It is a crucial information and must be stored in the client system as it is mandatory to provide it in any further step such as cancel or retrieve.
  name: id
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-hotel-order-schema.json
slug: hotel-booking-hotel-order
source_filename: hotel-booking-hotel-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-hotel-order-schema.json\",\n  \"title\": \"HotelOrder\",\n  \"description\": \"An Hotel Order is one or several hotel bookings done for a set of guest.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hotelBookings\": {\n      \"type\": \"array\",\n      \"uniqueItems\": true,\n      \"minItems\": 1,\n      \"description\": \"Array of hotel-bookings\",\n      \"items\": {\n        \"$ref\": \"#/definitions/HotelBooking\"\n      }\n    },\n    \"associatedRecords\": {\n      \"type\": \"array\",\n      \"uniqueItems\": false,\n      \"minItems\": 1,\n      \"description\": \"Reference and origin of the hotel order record\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"reference\": {\n            \"type\": \"string\",\n            \"\
  description\": \"Record locator of the PNR in which the hotel order is stored in Amadeus GDS.\",\n            \"example\": \"ABCDEF\",\n            \"minLength\": 6,\n            \"maxLength\": 6,\n            \"pattern\": \"^[A-Z0-9]{6}$\"\n          },\n          \"originSystemCode\": {\n            \"type\": \"string\",\n            \"minLength\": 1,\n            \"description\": \"As the reference is a PNR record locator, the originSystemCode is set to GDS.\",\n            \"example\": \"GDS\"\n          }\n        },\n        \"required\": [\n          \"reference\",\n          \"originSystemCode\"\n        ]\n      }\n    },\n    \"self\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"description\": \"Self URL for retrieving the Hotel Order\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"description\": \"Resource name - Is set to \\\"hotel-order\\\"\"\n    },\n    \"guests\": {\n      \"$ref\": \"#/definitions/Guests\"\n\
  \    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Id of the hotelorder. \\nIt is a crucial information and must be stored in the client system as it is mandatory to provide it in any further step such as cancel or retrieve.\",\n      \"minLength\": 1,\n      \"pattern\": \"[A-Za-z0-9+/=]\",\n      \"example\": \"12312\"\n    }\n  },\n  \"required\": [\n    \"hotelBookings\",\n    \"associatedRecords\",\n    \"self\",\n    \"type\",\n    \"guests\",\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-hotel-order-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: HotelOrder
---
