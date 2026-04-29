---
description: input parameter to create a flight order
layout: schema
name: FlightOrder
properties_list:
- description: the resource name
  name: type
  type: string
- description: unique identifier of the flight order
  name: id
  type: string
- description: office Id where to queue the order
  name: queuingOfficeId
  type: string
- description: office Id where will be transfered the ownership of the order
  name: ownerOfficeId
  type: string
- description: list of associated record
  name: associatedRecords
  type: array
- description: list of flight offer
  name: flightOffers
  type: array
- description: list of travelers
  name: travelers
  type: array
- description: ''
  name: remarks
  type: object
- description: list of form of payments
  name: formOfPayments
  type: array
- description: ''
  name: ticketingAgreement
  type: object
- description: list of automatic queuing
  name: automatedProcess
  type: array
- description: list of general contact information
  name: contacts
  type: array
- description: list of tickets
  name: tickets
  type: array
- description: list of forms of identifications applicable to travelers by airline
  name: formOfIdentifications
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-order-management-flightorder-schema.json
slug: flight-order-management-flightorder
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FlightOrder\",\n  \"description\": \"input parameter to create a flight order\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"the resource name\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"unique identifier of the flight order\"\n    },\n    \"queuingOfficeId\": {\n      \"type\": \"string\",\n      \"description\": \"office Id where to queue the order\"\n    },\n    \"ownerOfficeId\": {\n      \"type\": \"string\",\n      \"description\": \"office Id where will be transfered the ownership of the order\"\n    },\n    \"associatedRecords\": {\n      \"type\": \"array\",\n      \"description\": \"list of associated record\",\n      \"items\": {\n        \"$ref\": \"#/definitions/AssociatedRecord\"\n      }\n    },\n    \"flightOffers\": {\n      \"type\": \"array\",\n      \"description\": \"\
  list of flight offer\",\n      \"items\": {\n        \"$ref\": \"#/definitions/FlightOffer\"\n      }\n    },\n    \"travelers\": {\n      \"type\": \"array\",\n      \"description\": \"list of travelers\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Traveler\"\n      }\n    },\n    \"remarks\": {\n      \"$ref\": \"#/definitions/Remarks\"\n    },\n    \"formOfPayments\": {\n      \"type\": \"array\",\n      \"description\": \"list of form of payments\",\n      \"items\": {\n        \"$ref\": \"#/definitions/FormOfPayment\"\n      }\n    },\n    \"ticketingAgreement\": {\n      \"$ref\": \"#/definitions/TicketingAgreement\"\n    },\n    \"automatedProcess\": {\n      \"type\": \"array\",\n      \"description\": \"list of automatic queuing\",\n      \"items\": {\n        \"$ref\": \"#/definitions/AutomatedProcess\"\n      }\n    },\n    \"contacts\": {\n      \"type\": \"array\",\n      \"description\": \"list of general contact information\",\n      \"items\": {\n        \"\
  $ref\": \"#/definitions/Contact\"\n      }\n    },\n    \"tickets\": {\n      \"type\": \"array\",\n      \"description\": \"list of tickets\",\n      \"items\": {\n        \"$ref\": \"#/definitions/AirTravelDocument\"\n      }\n    },\n    \"formOfIdentifications\": {\n      \"type\": \"array\",\n      \"description\": \"list of forms of identifications applicable to travelers by airline\",\n      \"items\": {\n        \"$ref\": \"#/definitions/FormOfIdentification\"\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"flightOffers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-order-management-flightorder-schema.json
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
title: FlightOrder
---
