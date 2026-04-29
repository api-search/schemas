---
description: WeChatPayDetails schema from Adyen API
layout: schema
name: WeChatPayDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: '**wechatpay**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-we-chat-pay-details-schema.json
slug: checkout-we-chat-pay-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-we-chat-pay-details-schema.json\",\n  \"title\": \"WeChatPayDetails\",\n  \"description\": \"WeChatPayDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"wechatpay\",\n      \"description\": \"**wechatpay**\",\n      \"enum\": [\n        \"wechatpay\",\n        \"wechatpay_pos\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-we-chat-pay-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: WeChatPayDetails
---
