---
description: Contact Details
layout: schema
name: Hotel_Contact
properties_list:
- description: Phone Number
  name: phone
  type: string
- description: Fax Number
  name: fax
  type: string
- description: Email Address
  name: email
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-hotel_-contact-schema.json
slug: hotel-booking-hotel_-contact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-hotel_-contact-schema.json\",\n  \"title\": \"Hotel_Contact\",\n  \"description\": \"Contact Details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone Number\",\n      \"example\": \"+33679278416\",\n      \"minLength\": 2,\n      \"maxLength\": 90,\n      \"pattern\": \"^[+][1-9][0-9]{4,18}$\"\n    },\n    \"fax\": {\n      \"type\": \"string\",\n      \"description\": \"Fax Number\",\n      \"example\": \"+33679278417\",\n      \"minLength\": 2,\n      \"maxLength\": 90,\n      \"pattern\": \"^[+][1-9][0-9]{4,18}$\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email Address\",\n      \"format\": \"email\",\n      \"example\": \"hotel@brand.com\",\n      \"minLength\": 3,\n\
  \      \"maxLength\": 90,\n      \"pattern\": \"^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+.[a-zA-Z0-9-.]+$\"\n    }\n  },\n  \"required\": [\n    \"fax\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-hotel_-contact-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Hotel_Contact
---
