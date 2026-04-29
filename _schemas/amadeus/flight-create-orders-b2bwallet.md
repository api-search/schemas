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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-create-orders-b2bwallet-schema.json
slug: flight-create-orders-b2bwallet
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"B2bWallet\",\n  \"description\": \"b2b wallet\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardId\": {\n      \"type\": \"string\",\n      \"description\": \"card identifier\"\n    },\n    \"cardUsageName\": {\n      \"type\": \"string\",\n      \"description\": \"card usage name\"\n    },\n    \"cardFriendlyName\": {\n      \"type\": \"string\",\n      \"description\": \"card name\"\n    },\n    \"reportingData\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"virtualCreditCardDetails\": {\n      \"$ref\": \"#/definitions/VirtualCreditCardDetails\"\n    },\n    \"flightOfferIds\": {\n      \"type\": \"array\",\n      \"description\": \"Id of the concern\
  \ flightOffers\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-create-orders-b2bwallet-schema.json
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
title: B2bWallet
---
