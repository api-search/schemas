---
description: CheckoutNativeRedirectAction schema from Adyen API
layout: schema
name: CheckoutNativeRedirectAction
properties_list:
- description: When the redirect URL must be accessed via POST, use this data to post to the redirect URL.
  name: data
  type: object
- description: Specifies the HTTP method, for example GET or POST.
  name: method
  type: string
- description: Native SDK's redirect data containing the direct issuer link and state data that must be submitted to the /v1/nativeRedirect/redirectResult.
  name: nativeRedirectData
  type: string
- description: Specifies the payment method.
  name: paymentMethodType
  type: string
- description: '**nativeRedirect**'
  name: type
  type: string
- description: Specifies the URL to redirect to.
  name: url
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-checkout-native-redirect-action-schema.json
slug: checkout-checkout-native-redirect-action
source_filename: checkout-checkout-native-redirect-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-checkout-native-redirect-action-schema.json\",\n  \"title\": \"CheckoutNativeRedirectAction\",\n  \"description\": \"CheckoutNativeRedirectAction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"When the redirect URL must be accessed via POST, use this data to post to the redirect URL.\",\n      \"type\": \"object\"\n    },\n    \"method\": {\n      \"description\": \"Specifies the HTTP method, for example GET or POST.\",\n      \"type\": \"string\"\n    },\n    \"nativeRedirectData\": {\n      \"description\": \"Native SDK's redirect data containing the direct issuer link and state data that must be submitted to the /v1/nativeRedirect/redirectResult.\",\n      \"type\"\
  : \"string\"\n    },\n    \"paymentMethodType\": {\n      \"description\": \"Specifies the payment method.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"**nativeRedirect**\",\n      \"enum\": [\n        \"nativeRedirect\"\n      ],\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"description\": \"Specifies the URL to redirect to.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-checkout-native-redirect-action-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CheckoutNativeRedirectAction
---
