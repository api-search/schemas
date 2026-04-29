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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-order-management-formofidentification-schema.json
slug: flight-order-management-formofidentification
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FormOfIdentification\",\n  \"description\": \"alternative means of identifying stakeholders for eTicket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identificationType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of identification\",\n      \"enum\": [\n        \"DRIVERS_LICENSE\",\n        \"PASSPORT\",\n        \"NATIONAL_IDENTITY_CARD\",\n        \"BOOKING_CONFIRMATION\",\n        \"TICKET\",\n        \"OTHER_ID\"\n      ]\n    },\n    \"carrierCode\": {\n      \"type\": \"string\",\n      \"description\": \"providing the airline / carrier code\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"identification number relative to the type of identification either ticket number, booking number, passport number, identity card number, drivers licence number, other ID\"\n    },\n    \"travelerIds\": {\n      \"type\": \"array\",\n    \
  \  \"description\": \"Ids of the concerned travelers\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"flightOfferIds\": {\n      \"type\": \"array\",\n      \"description\": \"Id of the concerned flightOffers\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-order-management-formofidentification-schema.json
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: FormOfIdentification
---
