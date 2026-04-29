---
description: VisaCheckoutDetails schema from Adyen API
layout: schema
name: VisaCheckoutDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The funding source that should be used when multiple sources are available. For Brazilian combo cards, by default the funding source is credit. To use debit, set this value to **debit**.
  name: fundingSource
  type: string
- description: '**visacheckout**'
  name: type
  type: string
- description: The Visa Click to Pay Call ID value. When your shopper selects a payment and/or a shipping address from Visa Click to Pay, you will receive a Visa Click to Pay Call ID.
  name: visaCheckoutCallId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-visa-checkout-details-schema.json
slug: checkout-visa-checkout-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-visa-checkout-details-schema.json\",\n  \"title\": \"VisaCheckoutDetails\",\n  \"description\": \"VisaCheckoutDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"fundingSource\": {\n      \"description\": \"The funding source that should be used when multiple sources are available. For Brazilian combo cards, by default the funding source is credit. To use debit, set this value to **debit**.\",\n      \"enum\": [\n        \"credit\",\n        \"debit\"\n      ],\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"visacheckout\",\n      \"description\": \"**visacheckout**\",\n      \"enum\"\
  : [\n        \"visacheckout\"\n      ],\n      \"type\": \"string\"\n    },\n    \"visaCheckoutCallId\": {\n      \"description\": \"The Visa Click to Pay Call ID value. When your shopper selects a payment and/or a shipping address from Visa Click to Pay, you will receive a Visa Click to Pay Call ID.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"visaCheckoutCallId\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-visa-checkout-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: VisaCheckoutDetails
---
