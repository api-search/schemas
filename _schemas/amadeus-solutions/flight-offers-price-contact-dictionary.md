---
description: represents a contact
layout: schema
name: ContactDictionary
properties_list:
- description: the name of the person addressed by these contact details
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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-contact-dictionary-schema.json
slug: flight-offers-price-contact-dictionary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-contact-dictionary-schema.json\",\n  \"title\": \"ContactDictionary\",\n  \"description\": \"represents a contact\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"addresseeName\": {\n      \"description\": \"the name of the person addressed by these contact details\",\n      \"$ref\": \"#/definitions/Name\"\n    },\n    \"address\": {\n      \"$ref\": \"#/definitions/Address\"\n    },\n    \"language\": {\n      \"description\": \"the preferred language of communication with this Contact\",\n      \"type\": \"string\"\n    },\n    \"purpose\": {\n      \"$ref\": \"#/definitions/ContactPurpose\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-contact-dictionary-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: ContactDictionary
---
