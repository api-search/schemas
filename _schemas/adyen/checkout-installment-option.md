---
description: InstallmentOption schema from Adyen API
layout: schema
name: InstallmentOption
properties_list:
- description: The maximum number of installments offered for this payment method.
  name: maxValue
  type: integer
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
schema_file: json-schema/checkout-installment-option-schema.json
slug: checkout-installment-option
source_filename: checkout-installment-option-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-installment-option-schema.json\",\n  \"title\": \"InstallmentOption\",\n  \"description\": \"InstallmentOption schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxValue\": {\n      \"description\": \"The maximum number of installments offered for this payment method.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"plans\": {\n      \"x-addedInVersion\": \"64\",\n      \"description\": \"Defines the type of installment plan. If not set, defaults to **regular**.\\n\\nPossible values:\\n* **regular**\\n* **revolving**\",\n      \"items\": {\n        \"enum\": [\n          \"regular\",\n          \"revolving\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"preselectedValue\": {\n      \"x-addedInVersion\"\
  : \"64\",\n      \"description\": \"Preselected number of installments offered for this payment method.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"values\": {\n      \"x-addedInVersion\": \"64\",\n      \"description\": \"An array of the number of installments that the shopper can choose from. For example, **[2,3,5]**. This cannot be specified simultaneously with `maxValue`.\",\n      \"items\": {\n        \"format\": \"int32\",\n        \"type\": \"integer\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-installment-option-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: InstallmentOption
---
