---
description: extra equipment information
layout: schema
name: Equipment
properties_list:
- description: extra equipment codes, which can take following values code | name ------ | ------------------------------------- BBS | Baby stroller/Push chair BYC | Bicycle rack CBB | Cargo barrier rack CBF | Cargo
  name: code
  type: string
- description: extra equipment identifier
  name: itemId
  type: string
- description: extra equipment description
  name: description
  type: string
- description: ''
  name: quotation
  type: object
- description: ''
  name: converted
  type: object
- description: true if extra equipment is available for booking
  name: isBookable
  type: boolean
- description: true if tax included in extra equipment price
  name: taxIncluded
  type: boolean
- description: true if extra equipment price is included in total transfer amount
  name: includedInTotal
  type: boolean
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-equipment-schema.json
slug: transfer-booking-equipment
source_filename: transfer-booking-equipment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-equipment-schema.json\",\n  \"title\": \"Equipment\",\n  \"description\": \"extra equipment information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"extra equipment codes, which can take following values\\n\\ncode   | name                                 \\n------ | -------------------------------------  \\nBBS    | Baby stroller/Push chair\\nBYC    | Bicycle rack\\nCBB    | Cargo barrier rack\\nCBF    | Cargo barrier front\\nCBS    | Booster seat for child under 135cm or up to 12 years\\nCSB    | Child seat determined by weight/age of child 1-3 years / 9-18 Kg\\nCSI    | Child seat determined by weight/age of child 0-12 month/0-13Kg\\nCST    | Child seat determined by weight/age of child 4-7 years/15 \\u2013\
  \ 30 Kg\\nSBR    | Snow board racks\\nSKB    | Ski box\\nSKR    | Ski rack\\nTAB    | Travel Tablet \\nWAR    | Wheelchair access ramp\\nWHC    | Wheelchair\\nWIF    | Wi-Fi access\\nCNT    | Charger cable\\n\",\n      \"enum\": [\n        \"BBS\",\n        \"BYC\",\n        \"CBB\",\n        \"CBF\",\n        \"CBS\",\n        \"CSB\",\n        \"CSI\",\n        \"CST\",\n        \"SBR\",\n        \"SKB\",\n        \"SKR\",\n        \"TAB \",\n        \"WAR\",\n        \"WHC\",\n        \"WIF\",\n        \"CNT\"\n      ]\n    },\n    \"itemId\": {\n      \"type\": \"string\",\n      \"description\": \"extra equipment identifier\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"extra equipment description\"\n    },\n    \"quotation\": {\n      \"$ref\": \"#/definitions/Quotation\"\n    },\n    \"converted\": {\n      \"$ref\": \"#/definitions/Quotation\"\n    },\n    \"isBookable\": {\n      \"type\": \"boolean\",\n      \"description\": \"true if\
  \ extra equipment is available for booking\"\n    },\n    \"taxIncluded\": {\n      \"type\": \"boolean\",\n      \"description\": \"true if tax included in extra equipment price\"\n    },\n    \"includedInTotal\": {\n      \"type\": \"boolean\",\n      \"description\": \"true if extra equipment price is included in total transfer amount\"\n    }\n  },\n  \"required\": [\n    \"code\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-equipment-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Equipment
---
