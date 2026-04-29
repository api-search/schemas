---
description: ''
layout: schema
name: PredictionDataSuccess
properties_list:
- description: The card number for which the score is retrieved.
  name: customerPAN
  type: string
- description: Score data for the card numbers.
  name: scores
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-consumer-credit-analytics-prediction-data-success-schema.json
slug: mastercard-consumer-credit-analytics-prediction-data-success
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PredictionDataSuccess\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customerPAN\": {\n      \"type\": \"string\",\n      \"description\": \"The card number for which the score is retrieved.\"\n    },\n    \"scores\": {\n      \"type\": \"array\",\n      \"description\": \"Score data for the card numbers.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-consumer-credit-analytics-prediction-data-success-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: PredictionDataSuccess
---
