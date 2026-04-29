---
description: ''
layout: schema
name: OutSubscriptionInquiry
properties_list:
- description: 'Indicate to the ABU Integrator if they are subscribed to the inquired account. account number for a given merchant. *`subscribed: true`: Customer is subscribed. *`subscribed: false`: Customer is not s'
  name: subscribed
  type: boolean
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-automatic-billing-updater-out-subscription-inquiry-schema.json
slug: mastercard-automatic-billing-updater-out-subscription-inquiry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OutSubscriptionInquiry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subscribed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicate to the ABU Integrator if they are subscribed to the inquired account. account number for a given merchant. *`subscribed: true`: Customer is subscribed. *`subscribed: false`: Customer is not subscribed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-automatic-billing-updater-out-subscription-inquiry-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: OutSubscriptionInquiry
---
