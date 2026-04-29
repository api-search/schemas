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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-order-management-ticketingagreement-schema.json
slug: flight-order-management-ticketingagreement
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TicketingAgreement\",\n  \"description\": \"ticketing agreement\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"option\": {\n      \"$ref\": \"#/definitions/TicketingAgreementOption\"\n    },\n    \"delay\": {\n      \"type\": \"string\",\n      \"description\": \"Delay before applying automatic process if no issuance in days\"\n    },\n    \"dateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Exact date to apply automatic process if no issuance. YYYY-MM-DD format, e.g. 2019-06-07\"\n    },\n    \"segmentIds\": {\n      \"type\": \"array\",\n      \"description\": \"Ids of the impacted segments\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-order-management-ticketingagreement-schema.json
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
title: TicketingAgreement
---
