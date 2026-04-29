---
description: UpdatePaymentLinkRequest schema from Adyen API
layout: schema
name: UpdatePaymentLinkRequest
properties_list:
- description: 'Status of the payment link. Possible values: * **expired**'
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-update-payment-link-request-schema.json
slug: checkout-update-payment-link-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-update-payment-link-request-schema.json\",\n  \"title\": \"UpdatePaymentLinkRequest\",\n  \"description\": \"UpdatePaymentLinkRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"description\": \"Status of the payment link. Possible values:\\n* **expired**\",\n      \"enum\": [\n        \"expired\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-update-payment-link-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpdatePaymentLinkRequest
---
