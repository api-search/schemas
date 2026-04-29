---
description: Room Association represents a room booked in an hotel, the guests sleeping in this room, the hotel loyalty program if any, plus special request if any.
layout: schema
name: roomAssociation
properties_list:
- description: Array of guest references listing all the guests occupying the room. For each guest, the reference provided is the id also provided in guest section, except at booking creation time (in this only case
  name: guestReferences
  type: array
- description: special request to send to the reception (optional)
  name: specialRequest
  type: string
- description: Hotel offerID received in availability response, identifying the product to book.
  name: hotelOfferId
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-room-association-schema.json
slug: hotel-booking-room-association
source_filename: hotel-booking-room-association-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-room-association-schema.json\",\n  \"title\": \"roomAssociation\",\n  \"description\": \"Room Association represents a room booked in an hotel, the guests sleeping in this room, the hotel loyalty program if any, plus special request if any. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"guestReferences\": {\n      \"type\": \"array\",\n      \"description\": \"Array of guest references listing all the guests occupying the room.\\nFor each guest, the reference provided is the id also provided in guest section, except at booking creation time (in this only case, it will be a temporary id provided by the client called tid).\\nThe order of this list is important. The first one is the main guest, the one holding the reservation (and the form of payment).\\nThe following references\
  \ are the ones of the accompagnants, if any.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"guestReference\": {\n            \"type\": \"string\"\n          },\n          \"hotelLoyaltyId\": {\n            \"type\": \"string\",\n            \"description\": \"Hotel Chain Rewards Program Membership ID of the guest.\\nTo receive your Rewards Points, access online check in, fast check out. An error is returned by the Chain if the number is invalid.\\nExample Rewards Programs:\\n* Marriott Bonvoy\\n* Hilton Honors\\n* Hyatt Rewards\\n* IHG Rewards\\n* Wyndham Rewards\\n* Accor Live Limitless ALL\\n* Best Western Rewards\\n* Choice Privileges\\n* Radisson Rewards\\n\",\n            \"pattern\": \"^[A-Z0-9-]{1,21}$\",\n            \"minLength\": 1,\n            \"maxLength\": 21,\n            \"example\": \"3081031320523260\"\n          }\n        },\n        \"required\": [\n          \"guestReference\"\n        ]\n      }\n    },\n    \"specialRequest\"\
  : {\n      \"type\": \"string\",\n      \"minLength\": 2,\n      \"description\": \"special request to send to the reception (optional)\",\n      \"example\": \"TEST I will arrive at midnight\",\n      \"maxLength\": 120\n    },\n    \"hotelOfferId\": {\n      \"type\": \"string\",\n      \"description\": \"Hotel offerID received in availability response, identifying the product to book.\",\n      \"example\": \"63A93695B58821ABB0EC2B33FE9FAB24D72BF34B1BD7D707293763D8D9378FC3\",\n      \"maxLength\": 100,\n      \"minLength\": 2,\n      \"pattern\": \"^[A-Z0-9]*$\"\n    }\n  },\n  \"required\": [\n    \"guestReferences\",\n    \"hotelOfferId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-room-association-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: roomAssociation
---
