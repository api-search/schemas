---
description: PaymentDetailsRequest schema from Adyen API
layout: schema
name: PaymentDetailsRequest
properties_list:
- description: Data for 3DS authentication.
  name: authenticationData
  type: object
- description: Use this collection to submit the details that were returned as a result of the `/payments` call.
  name: details
  type: object
- description: Encoded payment data. For [authorizing a payment after using 3D Secure 2 Authentication-only](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only/#authorise-the-paymen
  name: paymentData
  type: string
- description: Change the `authenticationOnly` indicator originally set in the `/payments` request. Only needs to be set if you want to modify the value set previously.
  name: threeDSAuthenticationOnly
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-details-request-schema.json
slug: checkout-payment-details-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-details-request-schema.json\",\n  \"title\": \"PaymentDetailsRequest\",\n  \"description\": \"PaymentDetailsRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authenticationData\": {\n      \"x-addedInVersion\": \"69\",\n      \"description\": \"Data for 3DS authentication.\",\n      \"$ref\": \"#/components/schemas/DetailsRequestAuthenticationData\"\n    },\n    \"details\": {\n      \"description\": \"Use this collection to submit the details that were returned as a result of the `/payments` call.\",\n      \"$ref\": \"#/components/schemas/PaymentCompletionDetails\"\n    },\n    \"paymentData\": {\n      \"description\": \"Encoded payment data. For [authorizing a payment after using 3D Secure 2 Authentication-only](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only/#authorise-the-payment-with-adyen):\\\
  n\\nIf you received `resultCode`: **AuthenticationNotRequired** in the `/payments` response, use the `threeDSPaymentData` from the same response.\\n\\nIf you received `resultCode`: **AuthenticationFinished** in the `/payments` response, use the `action.paymentData` from the same response.\",\n      \"maxLength\": 200000,\n      \"type\": \"string\"\n    },\n    \"threeDSAuthenticationOnly\": {\n      \"x-addedInVersion\": \"40\",\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"69\",\n      \"x-deprecatedMessage\": \"Use `authenticationData.authenticationOnly` instead.\",\n      \"description\": \"Change the `authenticationOnly` indicator originally set in the `/payments` request. Only needs to be set if you want to modify the value set previously.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"details\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-details-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentDetailsRequest
---
