---
description: b2b wallet
layout: schema
name: B2bWallet
properties_list:
- description: card identifier
  name: cardId
  type: string
- description: card usage name
  name: cardUsageName
  type: string
- description: card name
  name: cardFriendlyName
  type: string
- description: ''
  name: reportingData
  type: array
- description: ''
  name: virtualCreditCardDetails
  type: object
- description: Id of the concern flightOffers
  name: flightOfferIds
  type: array
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-b2b-wallet-schema.json
slug: flight-create-orders-b2b-wallet
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-b2b-wallet-schema.json\",\n  \"title\": \"B2bWallet\",\n  \"description\": \"b2b wallet\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardId\": {\n      \"readOnly\": true,\n      \"description\": \"card identifier\",\n      \"type\": \"string\",\n      \"example\": \"1245365895336\"\n    },\n    \"cardUsageName\": {\n      \"description\": \"card usage name\",\n      \"type\": \"string\"\n    },\n    \"cardFriendlyName\": {\n      \"description\": \"card name\",\n      \"type\": \"string\",\n      \"example\": \"CB1\",\n      \"pattern\": \"[a-zA-Z0-9]{1,35}\"\n    },\n    \"reportingData\": {\n      \"type\": \"array\",\n      \"title\": \"reportingData\",\n      \"items\": {\n        \"title\": \"reportingData\",\n        \"type\": \"object\",\n        \"properties\"\
  : {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"reconcil1\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"example\": \"data1\"\n          }\n        }\n      }\n    },\n    \"virtualCreditCardDetails\": {\n      \"readOnly\": true,\n      \"$ref\": \"#/definitions/VirtualCreditCardDetails\"\n    },\n    \"flightOfferIds\": {\n      \"description\": \"Id of the concern flightOffers\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 6,\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": \"1\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-b2b-wallet-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: B2bWallet
---
