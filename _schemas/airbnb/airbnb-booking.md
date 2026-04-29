---
description: ''
layout: schema
name: Booking
properties_list:
- description: The unique identifier of the booking.
  name: id
  type: string
- description: The human-readable confirmation code for the booking.
  name: confirmation_code
  type: string
- description: The current status of the booking.
  name: status
  type: string
- description: The identifier of the booked experience.
  name: experience_id
  type: string
- description: The identifier of the booked schedule entry.
  name: schedule_id
  type: string
- description: ''
  name: guest
  type: object
- description: The number of guests included in the booking.
  name: guests_count
  type: integer
- description: The total price of the booking.
  name: total_price
  type: number
- description: The ISO 4217 currency code for the booking pricing.
  name: currency
  type: string
- description: The amount to be paid out to the host after fees.
  name: host_payout
  type: number
- description: The timestamp when the booking was created.
  name: created_at
  type: string
- description: The timestamp when the booking was last updated.
  name: updated_at
  type: string
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-booking-schema.json
slug: airbnb-booking
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-booking-schema.json\",\n  \"title\": \"Booking\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the booking.\"\n    },\n    \"confirmation_code\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable confirmation code for the booking.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the booking.\",\n      \"enum\": [\n        \"pending\",\n        \"confirmed\",\n        \"cancelled\",\n        \"completed\"\n      ]\n    },\n    \"experience_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the booked experience.\"\n    },\n    \"schedule_id\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The identifier of the booked schedule entry.\"\n    },\n    \"guest\": {\n      \"$ref\": \"#/components/schemas/BookingGuest\"\n    },\n    \"guests_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of guests included in the booking.\",\n      \"minimum\": 1\n    },\n    \"total_price\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The total price of the booking.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 4217 currency code for the booking pricing.\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"host_payout\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The amount to be paid out to the host after fees.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the booking was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"\
  string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the booking was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-booking-schema.json
tags: []
title: Booking
---
