---
description: quotation representing a price valuation and its components. The monetaryAmount at the root are the sum of base and all the taxes/fees/discounts
layout: schema
name: Quotation
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-quotation-schema.json
slug: transfer-booking-quotation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-quotation-schema.json\",\n  \"title\": \"Quotation\",\n  \"description\": \"quotation representing a price valuation and its components. The monetaryAmount at the root are the sum of base and all the taxes/fees/discounts\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/PointsAndCash\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"currencyCode\": {\n          \"type\": \"string\",\n          \"example\": \"USD\"\n        },\n        \"isEstimated\": {\n          \"type\": \"boolean\",\n          \"description\": \"indicates if the price is pre-estimated prior to ride. Becomes mandatory for transferType = TAXI\"\n        },\n        \"base\": {\n          \"description\": \"base price\",\n          \"allOf\": [\n            {\n           \
  \   \"$ref\": \"#/definitions/PointsAndCash\"\n            }\n          ]\n        },\n        \"discount\": {\n          \"description\": \"discount amount of base price\",\n          \"allOf\": [\n            {\n              \"$ref\": \"#/definitions/PointsAndCash\"\n            }\n          ]\n        },\n        \"taxes\": {\n          \"description\": \"Taxes breakdown\",\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/definitions/Tax\"\n          }\n        },\n        \"fees\": {\n          \"description\": \"Fees breakdown\",\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/definitions/Fee\"\n          }\n        },\n        \"totalTaxes\": {\n          \"$ref\": \"#/definitions/PointsAndCash\"\n        },\n        \"totalFees\": {\n          \"$ref\": \"#/definitions/PointsAndCash\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-quotation-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Quotation
---
