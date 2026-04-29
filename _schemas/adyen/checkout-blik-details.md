---
description: BlikDetails schema from Adyen API
layout: schema
name: BlikDetails
properties_list:
- description: BLIK code consisting of 6 digits.
  name: blikCode
  type: string
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: recurringDetailReference
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: storedPaymentMethodId
  type: string
- description: '**blik**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-blik-details-schema.json
slug: checkout-blik-details
source_filename: checkout-blik-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-blik-details-schema.json\",\n  \"title\": \"BlikDetails\",\n  \"description\": \"BlikDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"blikCode\": {\n      \"description\": \"BLIK code consisting of 6 digits.\",\n      \"type\": \"string\"\n    },\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"49\",\n      \"x-deprecatedMessage\": \"Use `storedPaymentMethodId` instead.\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"type\": \"string\"\n    },\n    \"storedPaymentMethodId\"\
  : {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"maxLength\": 64,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"**blik**\",\n      \"enum\": [\n        \"blik\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-blik-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BlikDetails
---
