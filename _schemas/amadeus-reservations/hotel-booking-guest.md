---
description: This modele represent a guest, his name, his loyalty programs, his age when it is a child...
layout: schema
name: Guest
properties_list:
- description: Airline frequent flyer of the guest /!\ In case of creation of a new hotel booking, only the first element of the array will be transmitted to the hotel provier. Please only provider one. In case of r
  name: frequentTraveler
  type: array
- description: Phone number of the guest It is recommanded to use the standard E.123 (https://en.wikipedia.org/wiki/E.123)
  name: phone
  type: string
- description: Email Adress of the guest
  name: email
  type: string
- description: Title/gender of the guest
  name: title
  type: string
- description: First Name (and middle name) of the guest. It is mandatory at create order but not mandatory at booking creation. - Complex pattern '^[A-Za-z \p{Han}\p{Katakana}\p{Hiragana}\p{Hangul}-]*$'
  name: firstName
  type: string
- description: 'Last name of the guest - It is mandatory at create order but not mandatory at booking creation. Complex pattern: ''^[A-Za-z \p{Han}\p{Katakana}\p{Hiragana}\p{Hangul}-]*$'''
  name: lastName
  type: string
- description: if the guest is a child, it is mandatory to provide a child age. Else the system will consider him as an adult
  name: childAge
  type: integer
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-guest-schema.json
slug: hotel-booking-guest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-guest-schema.json\",\n  \"title\": \"Guest\",\n  \"description\": \"This modele represent a guest, his name, his loyalty programs, his age when it is a child...\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"frequentTraveler\": {\n      \"type\": \"array\",\n      \"description\": \"Airline frequent flyer of the guest \\n/!\\\\ In case of creation of a new hotel booking, only the first element of the array will be transmitted to the hotel provier. Please only provider one.\\nIn case of retrieve of an hotel order, when a guest is having several frequent flyer numbers used in different hotel bookings, they will all be listed here.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"airlineCode\": {\n            \"type\": \"string\",\n\
  \            \"description\": \"Code of the Airline\",\n            \"example\": \"AF\",\n            \"minLength\": 2,\n            \"maxLength\": 3\n          },\n          \"frequentTravelerId\": {\n            \"type\": \"string\",\n            \"example\": \"32546971326\"\n          }\n        },\n        \"required\": [\n          \"airlineCode\",\n          \"frequentTravelerId\"\n        ]\n      }\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number of the guest\\n\\nIt is recommanded to use the standard E.123 (https://en.wikipedia.org/wiki/E.123)\",\n      \"maxLength\": 199,\n      \"minLength\": 2,\n      \"example\": \"+33679278416\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email Adress of the guest\",\n      \"pattern\": \"^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\\\\.[a-zA-Z0-9-.]+$\",\n      \"example\": \"test.test@test.com\",\n      \"maxLength\": 90,\n      \"minLength\": 3,\n      \"format\": \"\
  email\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title/gender of the guest\",\n      \"example\": \"MR\",\n      \"minLength\": 1,\n      \"maxLength\": 54,\n      \"pattern\": \"^[A-Za-z -]*$\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First Name (and middle name) of the guest. It is mandatory at create order but not mandatory at booking creation.\\n- Complex pattern '^[A-Za-z \\\\p{Han}\\\\p{Katakana}\\\\p{Hiragana}\\\\p{Hangul}-]*$' \\n\",\n      \"example\": \"TEST\",\n      \"maxLength\": 56,\n      \"minLength\": 1\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the guest - \\nIt is mandatory at create order but not mandatory at booking creation.\\nComplex pattern: '^[A-Za-z \\\\p{Han}\\\\p{Katakana}\\\\p{Hiragana}\\\\p{Hangul}-]*$' \",\n      \"example\": \"TEST\",\n      \"maxLength\": 57,\n      \"minLength\": 1\n    },\n    \"childAge\": {\n    \
  \  \"type\": \"integer\",\n      \"description\": \"if the guest is a child, it is mandatory to provide a child age. Else the system will consider him as an adult\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-guest-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Guest
---
