---
description: the information that are found on an ID document
layout: schema
name: Document
properties_list:
- description: The document number (shown on the document) . E.g. QFU514563221J
  name: number
  type: string
- description: Date at which the document has been issued.
  name: issuanceDate
  type: string
- description: Date after which the document is not valid anymore.
  name: expiryDate
  type: string
- description: '[ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) of the country that issued the document'
  name: issuanceCountry
  type: string
- description: A more precise information concerning the place where the document has been issued, when available. It may be a country, a state, a city or any other type of location. e.g. New-York
  name: issuanceLocation
  type: string
- description: '[ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) of the nationality appearing on the document'
  name: nationality
  type: string
- description: Birth place as indicated on the document
  name: birthPlace
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-price-document-schema.json
slug: flight-offers-price-document
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Document\",\n  \"description\": \"the information that are found on an ID document\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"The document number (shown on the document) . E.g. QFU514563221J\"\n    },\n    \"issuanceDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date at which the document has been issued.\"\n    },\n    \"expiryDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date after which the document is not valid anymore.\"\n    },\n    \"issuanceCountry\": {\n      \"type\": \"string\",\n      \"description\": \"[ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) of the country that issued the document\"\n    },\n    \"issuanceLocation\": {\n      \"type\": \"string\",\n      \"description\": \"A more precise\
  \ information concerning the place where the document has been issued, when available. It may be a country, a state, a city or any other type of location. e.g. New-York\"\n    },\n    \"nationality\": {\n      \"type\": \"string\",\n      \"description\": \"[ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) of the nationality appearing on the document\"\n    },\n    \"birthPlace\": {\n      \"type\": \"string\",\n      \"description\": \"Birth place as indicated on the document\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-price-document-schema.json
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
title: Document
---
