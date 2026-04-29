---
description: BillDeskDetails schema from Adyen API
layout: schema
name: BillDeskDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The issuer id of the shopper's selected bank.
  name: issuer
  type: string
- description: '**billdesk**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-bill-desk-details-schema.json
slug: checkout-bill-desk-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-bill-desk-details-schema.json\",\n  \"title\": \"BillDeskDetails\",\n  \"description\": \"BillDeskDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"issuer\": {\n      \"description\": \"The issuer id of the shopper's selected bank.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"**billdesk**\",\n      \"enum\": [\n        \"billdesk_online\",\n        \"billdesk_wallet\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"issuer\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-bill-desk-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BillDeskDetails
---
