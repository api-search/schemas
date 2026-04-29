---
description: TermAndCondition schema
layout: schema
name: TermAndCondition
properties_list:
- description: This defines what type of modification is concerned in this rule.
  name: category
  type: string
- description: ''
  name: circumstances
  type: string
- description: ''
  name: notApplicable
  type: boolean
- description: ''
  name: maxPenaltyAmount
  type: string
- description: ''
  name: descriptions
  type: array
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-term-and-condition-schema.json
slug: flight-offers-price-term-and-condition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-term-and-condition-schema.json\",\n  \"title\": \"TermAndCondition\",\n  \"description\": \"TermAndCondition schema\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"This defines what type of modification is concerned in this rule.\",\n      \"enum\": [\n        \"REFUND\",\n        \"EXCHANGE\",\n        \"REVALIDATION\",\n        \"REISSUE\",\n        \"REBOOK\",\n        \"CANCELLATION\"\n      ],\n      \"example\": \"EXCHANGE\"\n    },\n    \"circumstances\": {\n      \"type\": \"string\"\n    },\n    \"notApplicable\": {\n      \"type\": \"boolean\"\n    },\n    \"maxPenaltyAmount\": {\n      \"type\": \"string\"\n    },\n    \"descriptions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"title\": \"Description\"\
  ,\n        \"properties\": {\n          \"descriptionType\": {\n            \"type\": \"string\"\n          },\n          \"text\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-term-and-condition-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: TermAndCondition
---
