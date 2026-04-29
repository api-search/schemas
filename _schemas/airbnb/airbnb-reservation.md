---
description: ''
layout: schema
name: Reservation
properties_list:
- description: The unique identifier of the reservation.
  name: id
  type: string
- description: The human-readable confirmation code for the reservation.
  name: confirmation_code
  type: string
- description: The current status of the reservation.
  name: status
  type: string
- description: The identifier of the listing that was booked.
  name: listing_id
  type: string
- description: ''
  name: guest
  type: object
- description: The guest check-in date.
  name: check_in
  type: string
- description: The guest check-out date.
  name: check_out
  type: string
- description: The total number of nights in the reservation.
  name: nights
  type: integer
- description: The number of guests included in the reservation.
  name: guests_count
  type: integer
- description: The total price of the reservation in the listing currency.
  name: total_price
  type: number
- description: The ISO 4217 currency code for the reservation pricing.
  name: currency
  type: string
- description: The amount to be paid out to the host after fees.
  name: host_payout
  type: number
- description: The timestamp when the reservation was created.
  name: created_at
  type: string
- description: The timestamp when the reservation was last updated.
  name: updated_at
  type: string
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-reservation-schema.json
slug: airbnb-reservation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-reservation-schema.json\",\n  \"title\": \"Reservation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the reservation.\"\n    },\n    \"confirmation_code\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable confirmation code for the reservation.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the reservation.\",\n      \"enum\": [\n        \"pending\",\n        \"accepted\",\n        \"denied\",\n        \"cancelled\",\n        \"checked_in\",\n        \"checked_out\"\n      ]\n    },\n    \"listing_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the listing that was booked.\"\n    },\n    \"guest\"\
  : {\n      \"$ref\": \"#/components/schemas/Guest\"\n    },\n    \"check_in\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The guest check-in date.\"\n    },\n    \"check_out\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The guest check-out date.\"\n    },\n    \"nights\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of nights in the reservation.\",\n      \"minimum\": 1\n    },\n    \"guests_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of guests included in the reservation.\",\n      \"minimum\": 1\n    },\n    \"total_price\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The total price of the reservation in the listing currency.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 4217 currency code for the reservation pricing.\",\n      \"pattern\": \"^[A-Z]{3}$\"\
  \n    },\n    \"host_payout\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The amount to be paid out to the host after fees.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the reservation was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the reservation was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-reservation-schema.json
tags: []
title: Reservation
---
