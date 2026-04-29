---
description: CheckoutThreeDS2Action schema from Adyen API
layout: schema
name: CheckoutThreeDS2Action
properties_list:
- description: A token needed to authorise a payment.
  name: authorisationToken
  type: string
- description: Encoded payment data.
  name: paymentData
  type: string
- description: Specifies the payment method.
  name: paymentMethodType
  type: string
- description: A subtype of the token.
  name: subtype
  type: string
- description: A token to pass to the 3DS2 Component to get the fingerprint.
  name: token
  type: string
- description: '**threeDS2**'
  name: type
  type: string
- description: Specifies the URL to redirect to.
  name: url
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-checkout-three-ds2-action-schema.json
slug: checkout-checkout-three-ds2-action
source_filename: checkout-checkout-three-ds2-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-checkout-three-ds2-action-schema.json\",\n  \"title\": \"CheckoutThreeDS2Action\",\n  \"description\": \"CheckoutThreeDS2Action schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorisationToken\": {\n      \"description\": \"A token needed to authorise a payment.\",\n      \"type\": \"string\"\n    },\n    \"paymentData\": {\n      \"description\": \"Encoded payment data.\",\n      \"type\": \"string\"\n    },\n    \"paymentMethodType\": {\n      \"description\": \"Specifies the payment method.\",\n      \"type\": \"string\"\n    },\n    \"subtype\": {\n      \"description\": \"A subtype of the token.\",\n      \"type\": \"string\"\n    },\n    \"token\": {\n      \"description\": \"A token to pass to the 3DS2 Component to get the fingerprint.\",\n      \"type\": \"string\"\
  \n    },\n    \"type\": {\n      \"description\": \"**threeDS2**\",\n      \"enum\": [\n        \"threeDS2\"\n      ],\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"description\": \"Specifies the URL to redirect to.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-checkout-three-ds2-action-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CheckoutThreeDS2Action
---
