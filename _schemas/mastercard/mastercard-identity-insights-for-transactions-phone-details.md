---
description: ''
layout: schema
name: PhoneDetails
properties_list:
- description: Country code
  name: cc
  type: string
- description: Subscriber section of the number
  name: subscriber
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-phone-details-schema.json
slug: mastercard-identity-insights-for-transactions-phone-details
source_filename: mastercard-identity-insights-for-transactions-phone-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PhoneDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cc\": {\n      \"type\": \"string\",\n      \"description\": \"Country code\"\n    },\n    \"subscriber\": {\n      \"type\": \"string\",\n      \"description\": \"Subscriber section of the number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-phone-details-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: PhoneDetails
---
