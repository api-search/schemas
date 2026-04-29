---
description: ApplePaySessionResponse schema from Adyen API
layout: schema
name: ApplePaySessionResponse
properties_list:
- description: Base64 encoded data you need to [complete the Apple Pay merchant validation](https://docs.adyen.com/payment-methods/apple-pay/api-only?tab=adyen-certificate-validation_1#complete-apple-pay-session-val
  name: data
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-apple-pay-session-response-schema.json
slug: checkout-apple-pay-session-response
source_filename: checkout-apple-pay-session-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-apple-pay-session-response-schema.json\",\n  \"title\": \"ApplePaySessionResponse\",\n  \"description\": \"ApplePaySessionResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"Base64 encoded data you need to [complete the Apple Pay merchant validation](https://docs.adyen.com/payment-methods/apple-pay/api-only?tab=adyen-certificate-validation_1#complete-apple-pay-session-validation).\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-apple-pay-session-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ApplePaySessionResponse
---
