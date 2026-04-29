---
description: CheckoutSDKAction schema from Adyen API
layout: schema
name: CheckoutSDKAction
properties_list:
- description: Encoded payment data.
  name: paymentData
  type: string
- description: Specifies the payment method.
  name: paymentMethodType
  type: string
- description: The data to pass to the SDK.
  name: sdkData
  type: object
- description: The type of the action.
  name: type
  type: string
- description: Specifies the URL to redirect to.
  name: url
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-checkout-sdk-action-schema.json
slug: checkout-checkout-sdk-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-checkout-sdk-action-schema.json\",\n  \"title\": \"CheckoutSDKAction\",\n  \"description\": \"CheckoutSDKAction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"paymentData\": {\n      \"description\": \"Encoded payment data.\",\n      \"type\": \"string\"\n    },\n    \"paymentMethodType\": {\n      \"description\": \"Specifies the payment method.\",\n      \"type\": \"string\"\n    },\n    \"sdkData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The data to pass to the SDK.\",\n      \"type\": \"object\"\n    },\n    \"type\": {\n      \"description\": \"The type of the action.\",\n      \"enum\": [\n        \"sdk\",\n        \"wechatpaySDK\"\n      ],\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"description\"\
  : \"Specifies the URL to redirect to.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-checkout-sdk-action-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CheckoutSDKAction
---
