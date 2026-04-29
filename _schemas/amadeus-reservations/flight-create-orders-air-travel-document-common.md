---
description: AirTravelDocumentCommon schema
layout: schema
name: AirTravelDocumentCommon
properties_list:
- description: Type of the travel document
  name: documentType
  type: string
- description: Identifier of the travel document prefixed by its owner code [NALC - 3 digits]. Can either be a primary or a conjunctive document number. Necessary for TicketingReference definition.
  name: documentNumber
  type: string
- description: Status of the travel document contained in the fare element
  name: documentStatus
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-air-travel-document-common-schema.json
slug: flight-create-orders-air-travel-document-common
source_filename: flight-create-orders-air-travel-document-common-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-air-travel-document-common-schema.json\",\n  \"title\": \"AirTravelDocumentCommon\",\n  \"description\": \"AirTravelDocumentCommon schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"documentType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the travel document\",\n      \"enum\": [\n        \"ETICKET\",\n        \"PTICKET\",\n        \"EMD\",\n        \"MCO\"\n      ]\n    },\n    \"documentNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the travel document prefixed by its owner code [NALC - 3 digits]. Can either be a primary or a conjunctive document number. Necessary for TicketingReference definition.\"\n    },\n    \"documentStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the travel\
  \ document contained in the fare element\",\n      \"enum\": [\n        \"ISSUED\",\n        \"REFUNDED\",\n        \"VOID\",\n        \"ORIGINAL\",\n        \"EXCHANGED\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-air-travel-document-common-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: AirTravelDocumentCommon
---
