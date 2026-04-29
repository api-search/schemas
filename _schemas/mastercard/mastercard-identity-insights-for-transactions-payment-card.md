---
description: ''
layout: schema
name: PaymentCard
properties_list:
- description: Count of days since the payment card and name was first observed in the network. If they have not been observed together before, first seen days will be 0.
  name: cardHolderNamefirstSeenDays
  type: integer
- description: Count of times the payment card and name have been observed in the network over the past 90 days. If they have not been observed together in the past 90 days, velocity will be 0.
  name: cardHolderNameVelocity
  type: integer
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-payment-card-schema.json
slug: mastercard-identity-insights-for-transactions-payment-card
source_filename: mastercard-identity-insights-for-transactions-payment-card-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaymentCard\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardHolderNamefirstSeenDays\": {\n      \"type\": \"integer\",\n      \"description\": \"Count of days since the payment card and name was first observed in the network. If they have not been observed together before, first seen days will be 0.\"\n    },\n    \"cardHolderNameVelocity\": {\n      \"type\": \"integer\",\n      \"description\": \"Count of times the payment card and name have been observed in the network over the past 90 days. If they have not been observed together in the past 90 days, velocity will be 0.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-payment-card-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: PaymentCard
---
