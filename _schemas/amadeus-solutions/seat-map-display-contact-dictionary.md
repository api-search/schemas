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
- description: ''
  name: purpose
  type: object
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-contact-dictionary-schema.json
slug: seat-map-display-contact-dictionary
source_filename: seat-map-display-contact-dictionary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-contact-dictionary-schema.json\",\n  \"title\": \"ContactDictionary\",\n  \"description\": \"represents a contact\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"addresseeName\": {\n      \"description\": \"the name of the person addressed by these contact details\",\n      \"$ref\": \"#/definitions/Name\"\n    },\n    \"address\": {\n      \"$ref\": \"#/definitions/Address\"\n    },\n    \"purpose\": {\n      \"$ref\": \"#/definitions/ContactPurpose\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-contact-dictionary-schema.json
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
