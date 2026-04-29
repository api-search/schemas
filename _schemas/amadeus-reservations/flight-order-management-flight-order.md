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
- description: list of global remarks
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
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-flight-order-schema.json
slug: flight-order-management-flight-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-flight-order-schema.json\",\n  \"title\": \"FlightOrder\",\n  \"description\": \"input parameter to create a flight order\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"description\": \"the resource name\",\n      \"type\": \"string\",\n      \"example\": \"flight-order\"\n    },\n    \"id\": {\n      \"description\": \"unique identifier of the flight order\",\n      \"type\": \"string\",\n      \"example\": \"MlpZVkFMfFdBVFNPTnwyMDE1LTExLTAy\",\n      \"readOnly\": true\n    },\n    \"queuingOfficeId\": {\n      \"description\": \"office Id where to queue the order\",\n      \"type\": \"string\",\n      \"example\": \"NCE1A0955\"\n    },\n    \"ownerOfficeId\": {\n      \"description\": \"office Id where will be transfered the ownership of the order\"\
  ,\n      \"type\": \"string\",\n      \"example\": \"NCE1A0955\"\n    },\n    \"associatedRecords\": {\n      \"description\": \"list of associated record\",\n      \"type\": \"array\",\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/definitions/AssociatedRecord\"\n      }\n    },\n    \"flightOffers\": {\n      \"description\": \"list of flight offer\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 6,\n      \"items\": {\n        \"$ref\": \"#/definitions/FlightOffer\"\n      }\n    },\n    \"travelers\": {\n      \"description\": \"list of travelers\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 18,\n      \"items\": {\n        \"$ref\": \"#/definitions/Traveler\"\n      }\n    },\n    \"remarks\": {\n      \"description\": \"list of global remarks\",\n      \"$ref\": \"#/definitions/Remarks\"\n    },\n    \"formOfPayments\": {\n      \"description\": \"list of form of payments\",\n      \"type\": \"array\"\
  ,\n      \"minItems\": 1,\n      \"maxItems\": 6,\n      \"items\": {\n        \"$ref\": \"#/definitions/FormOfPayment\"\n      }\n    },\n    \"ticketingAgreement\": {\n      \"$ref\": \"#/definitions/TicketingAgreement\"\n    },\n    \"automatedProcess\": {\n      \"description\": \"list of automatic queuing\",\n      \"type\": \"array\",\n      \"minItems\": 0,\n      \"maxItems\": 31,\n      \"items\": {\n        \"$ref\": \"#/definitions/AutomatedProcess\"\n      }\n    },\n    \"contacts\": {\n      \"description\": \"list of general contact information\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Contact\"\n      }\n    },\n    \"tickets\": {\n      \"description\": \"list of tickets\",\n      \"readOnly\": true,\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/AirTravelDocument\"\n      }\n    },\n    \"formOfIdentifications\": {\n      \"description\": \"list of forms of identifications applicable to travelers\
  \ by airline\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/FormOfIdentification\"\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"flightOffers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-flight-order-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: FlightOrder
---
