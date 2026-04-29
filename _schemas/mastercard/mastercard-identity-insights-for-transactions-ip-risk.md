---
description: ''
layout: schema
name: IpRisk
properties_list:
- description: A 0-1 score (rounded to three decimal places) associated with an IP address.
  name: score
  type: number
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-ip-risk-schema.json
slug: mastercard-identity-insights-for-transactions-ip-risk
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IpRisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"score\": {\n      \"type\": \"number\",\n      \"description\": \"A 0-1 score (rounded to three decimal places) associated with an IP address.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-ip-risk-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: IpRisk
---
