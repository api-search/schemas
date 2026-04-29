---
description: information about corporation
layout: schema
name: Corporation
properties_list:
- description: ''
  name: address
  type: object
- description: 'corporate information map. Possible keys key | name ------ | ---------------------------- AU | Accounting Unit ON | Order Number DC | Department Code CC | Company Code CN | Company Name IA | Internal '
  name: info
  type: object
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-corporation-schema.json
slug: transfer-booking-corporation
source_filename: transfer-booking-corporation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-corporation-schema.json\",\n  \"title\": \"Corporation\",\n  \"description\": \"information about corporation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"$ref\": \"#/definitions/AddressCommon\"\n    },\n    \"info\": {\n      \"type\": \"object\",\n      \"description\": \"corporate information map. Possible keys\\n\\nkey    | name\\n------ | ----------------------------\\nAU\\t   | Accounting Unit\\nON\\t   | Order Number\\nDC\\t   | Department Code\\nCC\\t   | Company Code\\nCN\\t   | Company Name\\nIA\\t   | Internal Account\\nCE\\t   | Cost Centre\\nEN\\t   | Employee Number\\nPN\\t   | Project Number\\n\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"AU\": \"Accounting Unit\",\n \
  \       \"ON\": \"Order Number\",\n        \"DC\": \"Department Code\",\n        \"CC\": \"Company Code\",\n        \"CN\": \"Company Name\",\n        \"IA\": \"Internal Account\",\n        \"CE\": \"Cost Centre\",\n        \"EN\": \"Employee Number\",\n        \"PN\": \"Project Number\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-corporation-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Corporation
---
