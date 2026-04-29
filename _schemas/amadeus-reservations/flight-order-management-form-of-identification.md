---
description: alternative means of identifying stakeholders for eTicket.
layout: schema
name: FormOfIdentification
properties_list:
- description: Type of identification
  name: identificationType
  type: string
- description: providing the airline / carrier code
  name: carrierCode
  type: string
- description: identification number relative to the type of identification either ticket number, booking number, passport number, identity card number, drivers licence number, other ID
  name: number
  type: string
- description: Ids of the concerned travelers
  name: travelerIds
  type: array
- description: Id of the concerned flightOffers
  name: flightOfferIds
  type: array
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-form-of-identification-schema.json
slug: flight-order-management-form-of-identification
source_filename: flight-order-management-form-of-identification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-form-of-identification-schema.json\",\n  \"title\": \"FormOfIdentification\",\n  \"description\": \"alternative means of identifying stakeholders for eTicket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identificationType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of identification\",\n      \"enum\": [\n        \"DRIVERS_LICENSE\",\n        \"PASSPORT\",\n        \"NATIONAL_IDENTITY_CARD\",\n        \"BOOKING_CONFIRMATION\",\n        \"TICKET\",\n        \"OTHER_ID\"\n      ],\n      \"example\": \"PASSPORT\"\n    },\n    \"carrierCode\": {\n      \"type\": \"string\",\n      \"description\": \"providing the airline / carrier code\",\n      \"minLength\": 1,\n      \"maxLength\": 2,\n      \"example\": \"DL\"\n    },\n    \"number\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"identification number relative to the type of identification either ticket number, booking number, passport number, identity card number, drivers licence number, other ID\",\n      \"example\": \"XN0019390\"\n    },\n    \"travelerIds\": {\n      \"description\": \"Ids of the concerned travelers\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": \"1\"\n    },\n    \"flightOfferIds\": {\n      \"description\": \"Id of the concerned flightOffers\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 6,\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": \"1\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-form-of-identification-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: FormOfIdentification
---
