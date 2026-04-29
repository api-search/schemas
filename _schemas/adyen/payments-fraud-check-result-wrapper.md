---
description: FraudCheckResultWrapper schema from Adyen API
layout: schema
name: FraudCheckResultWrapper
properties_list:
- description: ''
  name: FraudCheckResult
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-fraud-check-result-wrapper-schema.json
slug: payments-fraud-check-result-wrapper
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-fraud-check-result-wrapper-schema.json\",\n  \"title\": \"FraudCheckResultWrapper\",\n  \"description\": \"FraudCheckResultWrapper schema from Adyen API\",\n  \"properties\": {\n    \"FraudCheckResult\": {\n      \"$ref\": \"#/components/schemas/FraudCheckResult\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-fraud-check-result-wrapper-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: FraudCheckResultWrapper
---
