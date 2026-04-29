---
description: information about provider
layout: schema
name: ServiceProvider
properties_list:
- description: provider code
  name: code
  type: string
- description: provider name
  name: name
  type: string
- description: URL to provider logo
  name: logoUrl
  type: string
- description: URL to provider's terms and conditions page
  name: termsUrl
  type: string
- description: indicates if sub-provider is preferred for the travel-seller
  name: isPreferred
  type: boolean
- description: ''
  name: contacts
  type: object
- description: list of provider settings
  name: settings
  type: array
- description: Information about the Customer stakeholder participating to the described sales summary.
  name: businessIdentification
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-serviceprovider-schema.json
slug: transfer-booking-serviceprovider
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ServiceProvider\",\n  \"description\": \"information about provider\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"provider code\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"provider name\"\n    },\n    \"logoUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL to provider logo\"\n    },\n    \"termsUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL to provider's terms and conditions page\"\n    },\n    \"isPreferred\": {\n      \"type\": \"boolean\",\n      \"description\": \"indicates if sub-provider is preferred for the travel-seller\"\n    },\n    \"contacts\": {\n      \"$ref\": \"#/definitions/ContactWithAddress\"\n    },\n    \"settings\": {\n      \"type\": \"array\",\n      \"description\": \"list of provider settings\",\n      \"items\": {\n    \
  \    \"type\": \"string\",\n        \"description\": \"provider setting\",\n        \"enum\": [\n          \"BILLING_ADDRESS_REQUIRED\",\n          \"FLIGHT_NUMBER_REQUIRED\",\n          \"CVV_NUMBER_REQUIRED\"\n        ]\n      }\n    },\n    \"businessIdentification\": {\n      \"description\": \"Information about the Customer stakeholder participating to the described sales summary.\",\n      \"properties\": {\n        \"vatRegistrationNumber\": {\n          \"type\": \"string\",\n          \"description\": \"VAT (Value Added Tax) Registration Number of the customer applicable ot the current sales.\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"code\",\n    \"name\",\n    \"logoUrl\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-booking-serviceprovider-schema.json
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
title: ServiceProvider
---
