---
description: ApplePaySessionRequest schema from Adyen API
layout: schema
name: ApplePaySessionRequest
properties_list:
- description: This is the name that your shoppers will see in the Apple Pay interface. The value returned as `configuration.merchantName` field from the [`/paymentMethods`](https://docs.adyen.com/api-explorer/#/Che
  name: displayName
  type: string
- description: The domain name you provided when you added Apple Pay in your Customer Area. This must match the `window.location.hostname` of the web shop.
  name: domainName
  type: string
- description: Your merchant identifier registered with Apple Pay. Use the value of the `configuration.merchantId` field from the [`/paymentMethods`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post
  name: merchantIdentifier
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-apple-pay-session-request-schema.json
slug: checkout-apple-pay-session-request
source_filename: checkout-apple-pay-session-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-apple-pay-session-request-schema.json\",\n  \"title\": \"ApplePaySessionRequest\",\n  \"description\": \"ApplePaySessionRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayName\": {\n      \"description\": \"This is the name that your shoppers will see in the Apple Pay interface.\\n\\nThe value returned as `configuration.merchantName` field from the [`/paymentMethods`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/paymentMethods) response.\",\n      \"type\": \"string\"\n    },\n    \"domainName\": {\n      \"description\": \"The domain name you provided when you added Apple Pay in your Customer Area.\\n\\nThis must match the `window.location.hostname` of the web shop.\",\n      \"type\": \"string\"\n    },\n    \"merchantIdentifier\": {\n   \
  \   \"description\": \"Your merchant identifier registered with Apple Pay.\\n\\nUse the value of the `configuration.merchantId` field from the [`/paymentMethods`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/paymentMethods) response.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"domainName\",\n    \"merchantIdentifier\",\n    \"displayName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-apple-pay-session-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ApplePaySessionRequest
---
