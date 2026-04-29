---
description: Restriction towards carriers.
layout: schema
name: CarrierRestrictions
properties_list:
- description: 'This flag enable/disable filtering of blacklisted airline by EU. The list of the banned airlines is published in the Official Journal of the European Union, where they are included as annexes A and B '
  name: blacklistedInEUAllowed
  type: boolean
- description: This option ensures that the system will only consider these airlines.
  name: excludedCarrierCodes
  type: array
- description: This option ensures that the system will only consider these airlines.
  name: includedCarrierCodes
  type: array
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-carrier-restrictions-schema.json
slug: flight-offers-search-carrier-restrictions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-carrier-restrictions-schema.json\",\n  \"title\": \"CarrierRestrictions\",\n  \"description\": \"Restriction towards carriers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"blacklistedInEUAllowed\": {\n      \"description\": \"This flag enable/disable filtering of blacklisted airline by EU. The list of the banned airlines is published in the Official Journal of the European Union, where they are included as annexes A and B to the Commission Regulation. The blacklist of an airline can concern all its flights or some specific aircraft types pertaining to the airline\",\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"excludedCarrierCodes\": {\n      \"description\": \"This option ensures that the system will only consider these airlines.\",\n      \"\
  type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 99,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"includedCarrierCodes\": {\n      \"description\": \"This option ensures that the system will only consider these airlines.\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 99,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-carrier-restrictions-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: CarrierRestrictions
---
