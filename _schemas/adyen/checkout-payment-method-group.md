---
description: PaymentMethodGroup schema from Adyen API
layout: schema
name: PaymentMethodGroup
properties_list:
- description: The name of the group.
  name: name
  type: string
- description: Echo data to be used if the payment method is displayed as part of this group.
  name: paymentMethodData
  type: string
- description: The unique code of the group.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-method-group-schema.json
slug: checkout-payment-method-group
source_filename: checkout-payment-method-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-method-group-schema.json\",\n  \"title\": \"PaymentMethodGroup\",\n  \"description\": \"PaymentMethodGroup schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"The name of the group.\",\n      \"type\": \"string\"\n    },\n    \"paymentMethodData\": {\n      \"description\": \"Echo data to be used if the payment method is displayed as part of this group.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The unique code of the group.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-method-group-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentMethodGroup
---
