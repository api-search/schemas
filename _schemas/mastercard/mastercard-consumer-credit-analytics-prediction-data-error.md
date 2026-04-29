---
description: ''
layout: schema
name: PredictionDataError
properties_list:
- description: The card number for which error is thrown
  name: customerPAN
  type: string
- description: List of errors for card number.
  name: errors
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-consumer-credit-analytics-prediction-data-error-schema.json
slug: mastercard-consumer-credit-analytics-prediction-data-error
source_filename: mastercard-consumer-credit-analytics-prediction-data-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PredictionDataError\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customerPAN\": {\n      \"type\": \"string\",\n      \"description\": \"The card number for which error is thrown\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of errors for card number.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-consumer-credit-analytics-prediction-data-error-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: PredictionDataError
---
