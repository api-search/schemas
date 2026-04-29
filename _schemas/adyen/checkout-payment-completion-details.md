---
description: PaymentCompletionDetails schema from Adyen API
layout: schema
name: PaymentCompletionDetails
properties_list:
- description: A payment session identifier returned by the card issuer.
  name: MD
  type: string
- description: (3D) Payment Authentication Request data for the card issuer.
  name: PaReq
  type: string
- description: (3D) Payment Authentication Response data by the card issuer.
  name: PaRes
  type: string
- description: ''
  name: authorization_token
  type: string
- description: PayPal-generated token for recurring payments.
  name: billingToken
  type: string
- description: The SMS verification code collected from the shopper.
  name: cupsecureplus.smscode
  type: string
- description: PayPal-generated third party access token.
  name: facilitatorAccessToken
  type: string
- description: A random number sent to the mobile phone number of the shopper to verify the payment.
  name: oneTimePasscode
  type: string
- description: PayPal-assigned ID for the order.
  name: orderID
  type: string
- description: PayPal-assigned ID for the payer (shopper).
  name: payerID
  type: string
- description: Payload appended to the `returnURL` as a result of the redirect.
  name: payload
  type: string
- description: PayPal-generated ID for the payment.
  name: paymentID
  type: string
- description: 'Value passed from the WeChat MiniProgram `wx.requestPayment` **complete** callback. Possible values: any value starting with `requestPayment:`.'
  name: paymentStatus
  type: string
- description: The result of the redirect as appended to the `returnURL`.
  name: redirectResult
  type: string
- description: Value you received from the WeChat Pay SDK.
  name: resultCode
  type: string
- description: 'Base64-encoded string returned by the Component after the challenge flow. It contains the following parameters: `transStatus`, `authorisationToken`.'
  name: threeDSResult
  type: string
- description: 'Base64-encoded string returned by the Component after the challenge flow. It contains the following parameter: `transStatus`.'
  name: threeds2.challengeResult
  type: string
- description: 'Base64-encoded string returned by the Component after the challenge flow. It contains the following parameter: `threeDSCompInd`.'
  name: threeds2.fingerprint
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-completion-details-schema.json
slug: checkout-payment-completion-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-completion-details-schema.json\",\n  \"title\": \"PaymentCompletionDetails\",\n  \"description\": \"PaymentCompletionDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MD\": {\n      \"description\": \"A payment session identifier returned by the card issuer.\",\n      \"maxLength\": 20000,\n      \"type\": \"string\"\n    },\n    \"PaReq\": {\n      \"description\": \"(3D) Payment Authentication Request data for the card issuer.\",\n      \"type\": \"string\"\n    },\n    \"PaRes\": {\n      \"description\": \"(3D) Payment Authentication Response data by the card issuer.\",\n      \"maxLength\": 20000,\n      \"type\": \"string\"\n    },\n    \"authorization_token\": {\n      \"type\": \"string\"\n    },\n    \"billingToken\": {\n      \"description\": \"PayPal-generated\
  \ token for recurring payments.\",\n      \"type\": \"string\"\n    },\n    \"cupsecureplus.smscode\": {\n      \"description\": \"The SMS verification code collected from the shopper.\",\n      \"type\": \"string\"\n    },\n    \"facilitatorAccessToken\": {\n      \"description\": \"PayPal-generated third party access token.\",\n      \"type\": \"string\"\n    },\n    \"oneTimePasscode\": {\n      \"description\": \"A random number sent to the mobile phone number of the shopper to verify the payment.\",\n      \"type\": \"string\"\n    },\n    \"orderID\": {\n      \"description\": \"PayPal-assigned ID for the order.\",\n      \"type\": \"string\"\n    },\n    \"payerID\": {\n      \"description\": \"PayPal-assigned ID for the payer (shopper).\",\n      \"type\": \"string\"\n    },\n    \"payload\": {\n      \"description\": \"Payload appended to the `returnURL` as a result of the redirect.\",\n      \"maxLength\": 20000,\n      \"type\": \"string\"\n    },\n    \"paymentID\": {\n   \
  \   \"description\": \"PayPal-generated ID for the payment.\",\n      \"type\": \"string\"\n    },\n    \"paymentStatus\": {\n      \"description\": \"Value passed from the WeChat MiniProgram `wx.requestPayment` **complete** callback. Possible values: any value starting with `requestPayment:`.\",\n      \"type\": \"string\"\n    },\n    \"redirectResult\": {\n      \"description\": \"The result of the redirect as appended to the `returnURL`.\",\n      \"maxLength\": 20000,\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"Value you received from the WeChat Pay SDK.\",\n      \"type\": \"string\"\n    },\n    \"threeDSResult\": {\n      \"description\": \"Base64-encoded string returned by the Component after the challenge flow. It contains the following parameters: `transStatus`, `authorisationToken`.\",\n      \"maxLength\": 50000,\n      \"type\": \"string\"\n    },\n    \"threeds2.challengeResult\": {\n      \"description\": \"Base64-encoded string\
  \ returned by the Component after the challenge flow. It contains the following parameter: `transStatus`.\",\n      \"maxLength\": 50000,\n      \"type\": \"string\"\n    },\n    \"threeds2.fingerprint\": {\n      \"description\": \"Base64-encoded string returned by the Component after the challenge flow. It contains the following parameter: `threeDSCompInd`.\",\n      \"maxLength\": 100000,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-completion-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentCompletionDetails
---
