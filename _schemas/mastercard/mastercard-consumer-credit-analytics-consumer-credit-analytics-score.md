---
description: ''
layout: schema
name: ConsumerCreditAnalyticsScore
properties_list:
- description: List of scores retrieved for the card numbers.
  name: predictionDataSuccesses
  type: array
- description: List of errors while retrieving the score for the card numbers.
  name: predictionDataErrors
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-consumer-credit-analytics-consumer-credit-analytics-score-schema.json
slug: mastercard-consumer-credit-analytics-consumer-credit-analytics-score
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConsumerCreditAnalyticsScore\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"predictionDataSuccesses\": {\n      \"type\": \"array\",\n      \"description\": \"List of scores retrieved for the card numbers.\"\n    },\n    \"predictionDataErrors\": {\n      \"type\": \"array\",\n      \"description\": \"List of errors while retrieving the score for the card numbers.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-consumer-credit-analytics-consumer-credit-analytics-score-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: ConsumerCreditAnalyticsScore
---
