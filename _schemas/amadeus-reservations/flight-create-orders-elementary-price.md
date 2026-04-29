---
description: elementaryPrice
layout: schema
name: ElementaryPrice
properties_list:
- description: Amount of the fare. could be alpha numeric. Ex- 500.20 or 514.13A, 'A'signifies additional collection.
  name: amount
  type: string
- description: Currency type of the fare.
  name: currencyCode
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-elementary-price-schema.json
slug: flight-create-orders-elementary-price
source_filename: flight-create-orders-elementary-price-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-elementary-price-schema.json\",\n  \"title\": \"ElementaryPrice\",\n  \"description\": \"elementaryPrice\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"string\",\n      \"description\": \"Amount of the fare. could be alpha numeric. Ex- 500.20 or 514.13A, 'A'signifies additional collection.\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Currency type of the fare.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-elementary-price-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: ElementaryPrice
---
