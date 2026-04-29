---
description: PaymentReversalRequest schema from Adyen API
layout: schema
name: PaymentReversalRequest
properties_list:
- description: Information about your application. For more details, see [Building Adyen solutions](https://docs.adyen.com/development-resources/building-adyen-solutions).
  name: applicationInfo
  type: object
- description: The merchant account that is used to process the payment.
  name: merchantAccount
  type: string
- description: 'Your reference for the reversal request. Maximum length: 80 characters.'
  name: reference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-reversal-request-schema.json
slug: checkout-payment-reversal-request
source_filename: checkout-payment-reversal-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-reversal-request-schema.json\",\n  \"title\": \"PaymentReversalRequest\",\n  \"description\": \"PaymentReversalRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationInfo\": {\n      \"description\": \"Information about your application. For more details, see [Building Adyen solutions](https://docs.adyen.com/development-resources/building-adyen-solutions).\",\n      \"$ref\": \"#/components/schemas/ApplicationInfo\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account that is used to process the payment.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the reversal request. Maximum length: 80 characters.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n\
  \    \"merchantAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-reversal-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentReversalRequest
---
