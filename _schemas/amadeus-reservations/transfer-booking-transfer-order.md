---
description: TransferOrder schema
layout: schema
name: TransferOrder
properties_list:
- description: the resource name
  name: type
  type: string
- description: transfer order identifier
  name: id
  type: string
- description: reference of the Trip e.g. YNK4JQ
  name: reference
  type: string
- description: transfer reservations, included in the order
  name: transfers
  type: array
- description: passengers, related to the Transfer Order
  name: passengers
  type: array
- description: ''
  name: agency
  type: object
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-transfer-order-schema.json
slug: transfer-booking-transfer-order
source_filename: transfer-booking-transfer-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-transfer-order-schema.json\",\n  \"title\": \"TransferOrder\",\n  \"description\": \"TransferOrder schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"description\": \"the resource name\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"transfer order identifier\"\n    },\n    \"reference\": {\n      \"type\": \"string\",\n      \"description\": \"reference of the Trip e.g. YNK4JQ\"\n    },\n    \"transfers\": {\n      \"type\": \"array\",\n      \"description\": \"transfer reservations, included in the order\",\n      \"items\": {\n        \"$ref\": \"#/definitions/TransferReservation\"\n      }\n    },\n    \"passengers\": {\n      \"type\": \"array\",\n      \"description\": \"passengers, related\
  \ to the Transfer Order\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Passenger\"\n      }\n    },\n    \"agency\": {\n      \"$ref\": \"#/definitions/Agency\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"id\",\n    \"transfers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-transfer-order-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: TransferOrder
---
