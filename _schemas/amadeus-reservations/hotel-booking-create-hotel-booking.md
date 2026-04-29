---
description: This model allows the creation of an hotel order.
layout: schema
name: CreateHotelBooking
properties_list:
- description: Optional information on the way the guest is arriving to the hotel. Today the application only supports Flight details.
  name: arrivalInformation
  type: object
- description: ''
  name: payment
  type: object
- description: Is to correlate a room to a guest and an offer.
  name: roomAssociations
  type: array
- description: Travel Agent details
  name: travelAgent
  type: object
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-create-hotel-booking-schema.json
slug: hotel-booking-create-hotel-booking
source_filename: hotel-booking-create-hotel-booking-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-create-hotel-booking-schema.json\",\n  \"title\": \"CreateHotelBooking\",\n  \"description\": \"This model allows the creation of an hotel order.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arrivalInformation\": {\n      \"type\": \"object\",\n      \"description\": \"Optional information on the way the guest is arriving to the hotel. Today the application only supports Flight details.\",\n      \"properties\": {\n        \"arrivalFlightDetails\": {\n          \"$ref\": \"#/definitions/ArrivalFlightDetails\"\n        }\n      }\n    },\n    \"payment\": {\n      \"$ref\": \"#/definitions/PaymentInput\"\n    },\n    \"roomAssociations\": {\n      \"type\": \"array\",\n      \"description\": \"Is to correlate a room to a guest and an offer.\",\n      \"maxItems\": 9,\n    \
  \  \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/definitions/roomAssociation\"\n      }\n    },\n    \"travelAgent\": {\n      \"type\": \"object\",\n      \"description\": \"Travel Agent details\",\n      \"required\": [\n        \"contact\"\n      ],\n      \"properties\": {\n        \"contact\": {\n          \"type\": \"object\",\n          \"required\": [\n            \"email\"\n          ],\n          \"properties\": {\n            \"email\": {\n              \"type\": \"string\",\n              \"example\": \"travelAgent@agency.com\",\n              \"minLength\": 3,\n              \"maxLength\": 90,\n              \"pattern\": \"^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+.[a-zA-Z0-9-.]+$\",\n              \"description\": \"travel agency email\"\n            },\n            \"fax\": {\n              \"type\": \"string\",\n              \"example\": \"+33985632145\",\n              \"minLength\": 2,\n              \"maxLength\": 90,\n              \"pattern\": \"^[+][1-9][0-9]{4,18}$\"\
  ,\n              \"description\": \"Even if this field is not mandatory it is recommended to fill it. This information is passed to the hotel provider. (When it is not provided in input, it is taken from the Office Profile of the Travel Agency).\"\n            },\n            \"phone\": {\n              \"type\": \"string\",\n              \"example\": \"+33679278416\",\n              \"minLength\": 2,\n              \"maxLength\": 199,\n              \"description\": \"Even if this field is not mandatory it is recommended to fill it. This information is always passed to the hotel provider. (When it is not provided in input, it is taken from the Office Profile of the Travel Agency).\"\n            }\n          }\n        },\n        \"travelAgentId\": {\n          \"type\": \"string\",\n          \"description\": \"Travel Agent ID also called Booking source or IATA number.\\nWhen received in request, it indicates that the travel agent wants to override the booking source receiving the\
  \ commission.\\nIf not provided, it is by default set to the IATA Number of the office profile the agent is connected to and who makes the booking. (the commission is given to that office) \"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"travelAgent\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-create-hotel-booking-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: CreateHotelBooking
---
