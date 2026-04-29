---
description: ''
layout: schema
name: EmailRiskScore
properties_list:
- description: Comprehensive risk score associated with an email address, with a higher score indicating a riskier individual. A number between 0 and 1 rounded to three decimal places.
  name: score
  type: number
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-email-risk-score-schema.json
slug: mastercard-identity-insights-for-transactions-email-risk-score
source_filename: mastercard-identity-insights-for-transactions-email-risk-score-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmailRiskScore\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"score\": {\n      \"type\": \"number\",\n      \"description\": \"Comprehensive risk score associated with an email address, with a higher score indicating a riskier individual.  A number between 0 and 1 rounded to three decimal places.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-email-risk-score-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: EmailRiskScore
---
