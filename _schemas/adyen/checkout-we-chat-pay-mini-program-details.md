---
description: WeChatPayMiniProgramDetails schema from Adyen API
layout: schema
name: WeChatPayMiniProgramDetails
properties_list:
- description: ''
  name: appId
  type: string
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: ''
  name: openid
  type: string
- description: '**wechatpayMiniProgram**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-we-chat-pay-mini-program-details-schema.json
slug: checkout-we-chat-pay-mini-program-details
source_filename: checkout-we-chat-pay-mini-program-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-we-chat-pay-mini-program-details-schema.json\",\n  \"title\": \"WeChatPayMiniProgramDetails\",\n  \"description\": \"WeChatPayMiniProgramDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appId\": {\n      \"type\": \"string\"\n    },\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"openid\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"wechatpayMiniProgram\",\n      \"description\": \"**wechatpayMiniProgram**\",\n      \"enum\": [\n        \"wechatpayMiniProgram\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-we-chat-pay-mini-program-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: WeChatPayMiniProgramDetails
---
