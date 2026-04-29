---
description: StandalonePaymentCancelResponse schema from Adyen API
layout: schema
name: StandalonePaymentCancelResponse
properties_list:
- description: The merchant account that is used to process the payment.
  name: merchantAccount
  type: string
- description: The [`reference`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__reqParam_reference) of the payment to cancel.
  name: paymentReference
  type: string
- description: Adyen's 16-character reference associated with the cancel request.
  name: pspReference
  type: string
- description: Your reference for the cancel request.
  name: reference
  type: string
- description: The status of your request. This will always have the value **received**.
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-standalone-payment-cancel-response-schema.json
slug: checkout-standalone-payment-cancel-response
source_filename: checkout-standalone-payment-cancel-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-standalone-payment-cancel-response-schema.json\",\n  \"title\": \"StandalonePaymentCancelResponse\",\n  \"description\": \"StandalonePaymentCancelResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantAccount\": {\n      \"description\": \"The merchant account that is used to process the payment.\",\n      \"type\": \"string\"\n    },\n    \"paymentReference\": {\n      \"description\": \"The [`reference`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__reqParam_reference) of the payment to cancel.\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"Adyen's 16-character reference associated with the cancel request.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\":\
  \ \"Your reference for the cancel request.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of your request. This will always have the value **received**.\",\n      \"enum\": [\n        \"received\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"merchantAccount\",\n    \"pspReference\",\n    \"paymentReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-standalone-payment-cancel-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StandalonePaymentCancelResponse
---
