---
description: price information
layout: schema
name: Extended_Price
properties_list: []
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-extended_-price-schema.json
slug: flight-offers-price-extended_-price
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-extended_-price-schema.json\",\n  \"title\": \"Extended_Price\",\n  \"description\": \"price information\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"margin\": {\n          \"description\": \"BOOK step ONLY - The price margin percentage (plus or minus) that the booking can tolerate. When set to 0, then no price magin is tolerated.\",\n          \"type\": \"string\",\n          \"example\": \"1.00\"\n        },\n        \"grandTotal\": {\n          \"description\": \"Total amount paid by the user (including fees and selected additional services).\",\n          \"type\": \"string\",\n          \"example\": \"987.00\"\n        },\n        \"billingCurrency\": {\n          \"description\": \"Currency of the payment.\
  \ It may be different than the requested currency\",\n          \"type\": \"string\",\n          \"example\": \"EUR\"\n        },\n        \"additionalServices\": {\n          \"type\": \"array\",\n          \"title\": \"AdditionalServices\",\n          \"items\": {\n            \"title\": \"AdditionalService\",\n            \"type\": \"object\",\n            \"properties\": {\n              \"amount\": {\n                \"type\": \"string\",\n                \"example\": \"332.70\"\n              },\n              \"type\": {\n                \"$ref\": \"#/definitions/AdditionalServiceType\"\n              }\n            }\n          }\n        }\n      }\n    },\n    {\n      \"$ref\": \"#/definitions/Price\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-extended_-price-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Extended_Price
---
