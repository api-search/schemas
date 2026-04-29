---
description: ticketing agreement
layout: schema
name: TicketingAgreement
properties_list:
- description: ''
  name: option
  type: object
- description: Delay before applying automatic process if no issuance in days
  name: delay
  type: string
- description: Exact date to apply automatic process if no issuance. YYYY-MM-DD format, e.g. 2019-06-07
  name: dateTime
  type: string
- description: Ids of the impacted segments
  name: segmentIds
  type: array
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-ticketing-agreement-schema.json
slug: flight-order-management-ticketing-agreement
source_filename: flight-order-management-ticketing-agreement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-ticketing-agreement-schema.json\",\n  \"title\": \"TicketingAgreement\",\n  \"description\": \"ticketing agreement\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"option\": {\n      \"$ref\": \"#/definitions/TicketingAgreementOption\"\n    },\n    \"delay\": {\n      \"description\": \"Delay before applying automatic process if no issuance in days\",\n      \"type\": \"string\"\n    },\n    \"dateTime\": {\n      \"description\": \"Exact date to apply automatic process if no issuance. YYYY-MM-DD format, e.g. 2019-06-07\",\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"example\": \"2017-10-23\"\n    },\n    \"segmentIds\": {\n      \"description\": \"Ids of the impacted segments\",\n      \"type\": \"array\",\n      \"readOnly\": true,\n      \"items\"\
  : {\n        \"type\": \"string\"\n      },\n      \"example\": \"1\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-ticketing-agreement-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: TicketingAgreement
---
