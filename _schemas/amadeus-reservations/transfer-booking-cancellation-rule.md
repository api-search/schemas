---
description: cancellation rule information
layout: schema
name: CancellationRule
properties_list:
- description: description of cancellation rule
  name: ruleDescription
  type: string
- description: type of fee - percentage of total amount (PERCENTAGE) or fixed amount (VALUE)
  name: feeType
  type: string
- description: value of the fee, e.g. "100" or "12.50"
  name: feeValue
  type: string
- description: currency code of the fee in [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) format, e.g. USD, EUR
  name: currencyCode
  type: string
- description: type of metric
  name: metricType
  type: string
- description: metric min value
  name: metricMin
  type: string
- description: metric max value
  name: metricMax
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-cancellation-rule-schema.json
slug: transfer-booking-cancellation-rule
source_filename: transfer-booking-cancellation-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-cancellation-rule-schema.json\",\n  \"title\": \"CancellationRule\",\n  \"description\": \"cancellation rule information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ruleDescription\": {\n      \"type\": \"string\",\n      \"description\": \"description of cancellation rule\"\n    },\n    \"feeType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PERCENTAGE\",\n        \"VALUE\"\n      ],\n      \"description\": \"type of fee - percentage of total amount (PERCENTAGE) or fixed amount (VALUE)\\n\"\n    },\n    \"feeValue\": {\n      \"type\": \"string\",\n      \"description\": \"value of the fee, e.g. \\\"100\\\" or \\\"12.50\\\"\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"pattern\": \"[A-Z]{3}\",\n      \"description\": \"currency\
  \ code of the fee in [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) format, e.g. USD, EUR\"\n    },\n    \"metricType\": {\n      \"type\": \"string\",\n      \"description\": \"type of metric\",\n      \"enum\": [\n        \"MINUTES\",\n        \"HOURS\",\n        \"DAYS\",\n        \"YEARS\"\n      ]\n    },\n    \"metricMin\": {\n      \"type\": \"string\",\n      \"description\": \"metric min value\"\n    },\n    \"metricMax\": {\n      \"type\": \"string\",\n      \"description\": \"metric max value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-cancellation-rule-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: CancellationRule
---
