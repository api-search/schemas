---
description: PaymentMethodIssuer schema from Adyen API
layout: schema
name: PaymentMethodIssuer
properties_list:
- description: A boolean value indicating whether this issuer is unavailable. Can be `true` whenever the issuer is offline.
  name: disabled
  type: boolean
- description: The unique identifier of this issuer, to submit in requests to /payments.
  name: id
  type: string
- description: A localized name of the issuer.
  name: name
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-method-issuer-schema.json
slug: checkout-payment-method-issuer
source_filename: checkout-payment-method-issuer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-method-issuer-schema.json\",\n  \"title\": \"PaymentMethodIssuer\",\n  \"description\": \"PaymentMethodIssuer schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disabled\": {\n      \"default\": false,\n      \"description\": \"A boolean value indicating whether this issuer is unavailable. Can be `true` whenever the issuer is offline.\",\n      \"type\": \"boolean\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of this issuer, to submit in requests to /payments.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"A localized name of the issuer.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-method-issuer-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentMethodIssuer
---
