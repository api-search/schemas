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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-search-carrierrestrictions-schema.json
slug: flight-offers-search-carrierrestrictions
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CarrierRestrictions\",\n  \"description\": \"Restriction towards carriers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"blacklistedInEUAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"This flag enable/disable filtering of blacklisted airline by EU. The list of the banned airlines is published in the Official Journal of the European Union, where they are included as annexes A and B to the Commission Regulation. The blacklist of an airline can concern all its flights or some specific aircraft types pertaining to the airline\"\n    },\n    \"excludedCarrierCodes\": {\n      \"type\": \"array\",\n      \"description\": \"This option ensures that the system will only consider these airlines.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"includedCarrierCodes\": {\n      \"type\": \"array\",\n      \"description\": \"This option ensures that\
  \ the system will only consider these airlines.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-search-carrierrestrictions-schema.json
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
title: CarrierRestrictions
---
