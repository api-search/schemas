---
description: represents a contact
layout: schema
name: ContactDictionary
properties_list:
- description: ''
  name: addresseeName
  type: object
- description: ''
  name: address
  type: object
- description: the preferred language of communication with this Contact
  name: language
  type: string
- description: ''
  name: purpose
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-create-orders-contactdictionary-schema.json
slug: flight-create-orders-contactdictionary
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ContactDictionary\",\n  \"description\": \"represents a contact\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"addresseeName\": {\n      \"$ref\": \"#/definitions/Name\"\n    },\n    \"address\": {\n      \"$ref\": \"#/definitions/Address\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"the preferred language of communication with this Contact\"\n    },\n    \"purpose\": {\n      \"$ref\": \"#/definitions/ContactPurpose\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-create-orders-contactdictionary-schema.json
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
title: ContactDictionary
---
