---
description: ''
layout: schema
name: PaymentAmount
properties_list:
- description: A ratio of the purchase amount compared to the median purchase amount seen for other similar merchants in the same category. The higher the ratio means that the purchase amount is further from the med
  name: merchantCategoryRatio
  type: number
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-payment-amount-schema.json
slug: mastercard-identity-insights-for-transactions-payment-amount
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaymentAmount\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantCategoryRatio\": {\n      \"type\": \"number\",\n      \"description\": \"A ratio of the purchase amount compared to the median purchase amount seen for other similar merchants in the same category. The higher the ratio means that the purchase amount is further from the median purchase amount observed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-payment-amount-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: PaymentAmount
---
