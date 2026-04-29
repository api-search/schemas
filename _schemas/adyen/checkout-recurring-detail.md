---
description: RecurringDetail schema from Adyen API
layout: schema
name: RecurringDetail
properties_list:
- description: 'Brand for the selected gift card. For example: plastix, hmclub.'
  name: brand
  type: string
- description: 'List of possible brands. For example: visa, mc.'
  name: brands
  type: array
- description: The configuration of the payment method.
  name: configuration
  type: object
- description: The funding source of the payment method.
  name: fundingSource
  type: string
- description: The group where this payment method belongs to.
  name: group
  type: object
- description: All input details to be provided to complete the payment with this payment method.
  name: inputDetails
  type: array
- description: A list of issuers for this payment method.
  name: issuers
  type: array
- description: The displayable name of this payment method.
  name: name
  type: string
- description: The reference that uniquely identifies the recurring detail.
  name: recurringDetailReference
  type: string
- description: Contains information on previously stored payment details.
  name: storedDetails
  type: object
- description: The unique payment method code.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-recurring-detail-schema.json
slug: checkout-recurring-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-recurring-detail-schema.json\",\n  \"title\": \"RecurringDetail\",\n  \"description\": \"RecurringDetail schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand\": {\n      \"x-addedInVersion\": \"65\",\n      \"description\": \"Brand for the selected gift card. For example: plastix, hmclub.\",\n      \"type\": \"string\"\n    },\n    \"brands\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"List of possible brands. For example: visa, mc.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"configuration\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The configuration of the payment method.\",\n      \"type\": \"object\"\n    },\n    \"fundingSource\"\
  : {\n      \"x-addedInVersion\": \"53\",\n      \"description\": \"The funding source of the payment method.\",\n      \"enum\": [\n        \"credit\",\n        \"debit\"\n      ],\n      \"type\": \"string\"\n    },\n    \"group\": {\n      \"description\": \"The group where this payment method belongs to.\",\n      \"$ref\": \"#/components/schemas/PaymentMethodGroup\"\n    },\n    \"inputDetails\": {\n      \"deprecated\": true,\n      \"description\": \"All input details to be provided to complete the payment with this payment method.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/InputDetail\"\n      },\n      \"type\": \"array\"\n    },\n    \"issuers\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"A list of issuers for this payment method.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PaymentMethodIssuer\"\n      },\n      \"type\": \"array\"\n    },\n    \"name\": {\n      \"description\": \"The displayable name of this payment\
  \ method.\",\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"description\": \"The reference that uniquely identifies the recurring detail.\",\n      \"type\": \"string\"\n    },\n    \"storedDetails\": {\n      \"description\": \"Contains information on previously stored payment details.\",\n      \"$ref\": \"#/components/schemas/StoredDetails\"\n    },\n    \"type\": {\n      \"description\": \"The unique payment method code.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-recurring-detail-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RecurringDetail
---
