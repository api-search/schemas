---
description: CheckoutSessionInstallmentOption schema from Adyen API
layout: schema
name: CheckoutSessionInstallmentOption
properties_list:
- description: 'Defines the type of installment plan. If not set, defaults to **regular**. Possible values: * **regular** * **revolving**'
  name: plans
  type: array
- description: Preselected number of installments offered for this payment method.
  name: preselectedValue
  type: integer
- description: An array of the number of installments that the shopper can choose from. For example, **[2,3,5]**. This cannot be specified simultaneously with `maxValue`.
  name: values
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-checkout-session-installment-option-schema.json
slug: checkout-checkout-session-installment-option
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-checkout-session-installment-option-schema.json\",\n  \"title\": \"CheckoutSessionInstallmentOption\",\n  \"description\": \"CheckoutSessionInstallmentOption schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"plans\": {\n      \"description\": \"Defines the type of installment plan. If not set, defaults to **regular**.\\n\\nPossible values:\\n* **regular**\\n* **revolving**\",\n      \"items\": {\n        \"enum\": [\n          \"regular\",\n          \"revolving\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"preselectedValue\": {\n      \"description\": \"Preselected number of installments offered for this payment method.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"values\": {\n      \"description\"\
  : \"An array of the number of installments that the shopper can choose from. For example, **[2,3,5]**. This cannot be specified simultaneously with `maxValue`.\",\n      \"items\": {\n        \"format\": \"int32\",\n        \"type\": \"integer\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-checkout-session-installment-option-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CheckoutSessionInstallmentOption
---
