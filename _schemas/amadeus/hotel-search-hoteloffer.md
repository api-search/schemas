---
description: Hotel Offer
layout: schema
name: HotelOffer
properties_list:
- description: ''
  name: type
  type: object
- description: Unique identifier of this offer. Might be valid for a temporary period only.
  name: id
  type: string
- description: check-in date of the stay (hotel local date). Format YYYY-MM-DD The lowest accepted value is today date (no dates in the past).
  name: checkInDate
  type: string
- description: check-out date of the stay (hotel local date). Format YYYY-MM-DD The lowest accepted value is `checkInDate`+1.
  name: checkOutDate
  type: string
- description: number of rooms (1-9)
  name: roomQuantity
  type: string
- description: Special Rate - Provider Response Code (3 chars) Examples * RAC - Rack * BAR - Best Available Rate * PRO - Promotional * COR - Corporate * GOV - Government (qualified) * AAA - AAA (qualified) * BNB - B
  name: rateCode
  type: string
- description: ''
  name: rateFamilyEstimated
  type: object
- description: 'Special Rate Category Examples: ASSOCIATION FAMILY_PLAN'
  name: category
  type: string
- description: ''
  name: description
  type: object
- description: ''
  name: commission
  type: object
- description: ''
  name: boardType
  type: object
- description: ''
  name: room
  type: object
- description: ''
  name: guests
  type: object
- description: ''
  name: price
  type: object
- description: ''
  name: policies
  type: object
- description: A self link to the object. Use this to refresh the Offer price
  name: self
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hoteloffer-schema.json
slug: hotel-search-hoteloffer
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelOffer\",\n  \"description\": \"Hotel Offer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"$ref\": \"#/definitions/Type\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of this offer. Might be valid for a temporary period only.\"\n    },\n    \"checkInDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"check-in date of the stay (hotel local date). Format YYYY-MM-DD\\nThe lowest accepted value is today date (no dates in the past).\"\n    },\n    \"checkOutDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"check-out date of the stay (hotel local date). Format YYYY-MM-DD\\nThe lowest accepted value is `checkInDate`+1.\"\n    },\n    \"roomQuantity\": {\n      \"type\": \"string\",\n      \"description\": \"number of rooms (1-9)\"\n    },\n\
  \    \"rateCode\": {\n      \"type\": \"string\",\n      \"description\": \"Special Rate - Provider Response Code (3 chars)\\nExamples\\n\\n  * RAC - Rack\\n\\n  * BAR - Best Available Rate\\n\\n  * PRO - Promotional\\n\\n  * COR - Corporate\\n\\n  * GOV - Government (qualified)\\n\\n  * AAA - AAA (qualified)\\n\\n  * BNB - Bed and Breakfast\\n\\n  * PKG - Package\\n\\n  * TVL - Travel Industry\\n\\n  * SPC - Special Promo Rate\\n\\n  * WKD - Weekend\\n\\n  * CON - Convention\\n\\n  * SNR - Senior (Europe) (qualified)\\n\\n  * ARP - AARP - American Association of Retired People (50+) (qualified)\\n\\n  * SRS - Senior (qualified)\\n\\n  * ROR - Room Only Rate (no breakfast)\\n\\n  * FAM - Family\\n\\n  * DAY - Day rate\"\n    },\n    \"rateFamilyEstimated\": {\n      \"$ref\": \"#/definitions/HotelProduct_RateFamily\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Special Rate Category\\nExamples:\\n  ASSOCIATION\\n  FAMILY_PLAN\"\n    },\n    \"description\"\
  : {\n      \"$ref\": \"#/definitions/QualifiedFreeText\"\n    },\n    \"commission\": {\n      \"$ref\": \"#/definitions/HotelProduct_Commission\"\n    },\n    \"boardType\": {\n      \"$ref\": \"#/definitions/BoardType\"\n    },\n    \"room\": {\n      \"$ref\": \"#/definitions/HotelProduct_RoomDetails\"\n    },\n    \"guests\": {\n      \"$ref\": \"#/definitions/HotelProduct_Guests\"\n    },\n    \"price\": {\n      \"$ref\": \"#/definitions/HotelProduct_HotelPrice\"\n    },\n    \"policies\": {\n      \"$ref\": \"#/definitions/HotelProduct_PolicyDetails\"\n    },\n    \"self\": {\n      \"type\": \"string\",\n      \"description\": \"A self link to the object. Use this to refresh the Offer price\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"rateCode\",\n    \"room\",\n    \"price\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hoteloffer-schema.json
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
title: HotelOffer
---
