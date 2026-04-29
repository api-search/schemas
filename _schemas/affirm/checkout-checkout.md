---
description: Represents an Affirm checkout session with full order details, customer information, and current checkout status.
layout: schema
name: Checkout
properties_list:
- description: Unique identifier for this checkout session.
  name: checkout_id
  type: string
- description: Current status of the checkout session.
  name: checkout_status
  type: string
- description: The checkout flow type used for this session.
  name: checkout_flow_type
  type: string
- description: ISO 4217 currency code for the checkout.
  name: currency
  type: string
- description: Total checkout amount in cents.
  name: total
  type: integer
- description: Shipping cost in cents.
  name: shipping_amount
  type: integer
- description: Tax amount in cents.
  name: tax_amount
  type: integer
- description: Merchant's internal order identifier.
  name: order_id
  type: string
- description: Internal financing program identifier applied to this checkout.
  name: financial_program_name
  type: string
- description: Customer-facing financing program name.
  name: financial_program_external_name
  type: string
- description: Loan billing frequency for the financing applied.
  name: billing_frequency
  type: string
- description: Version of the Affirm API used to create this checkout.
  name: api_version
  type: string
- description: Product category associated with this checkout, if set.
  name: product_type
  type: string
- description: ''
  name: billing
  type: object
- description: ''
  name: shipping
  type: object
- description: ''
  name: merchant
  type: object
- description: Additional checkout metadata.
  name: metadata
  type: object
- description: Affirm internal tracking information.
  name: meta
  type: object
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/checkout-checkout-schema.json
slug: checkout-checkout
source_filename: checkout-checkout-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-checkout-schema.json\",\n  \"title\": \"Checkout\",\n  \"description\": \"Represents an Affirm checkout session with full order details, customer information, and current checkout status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkout_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this checkout session.\",\n      \"example\": \"500123\"\n    },\n    \"checkout_status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the checkout session.\",\n      \"enum\": [\n        \"pending\",\n        \"confirmed\",\n        \"failed\",\n        \"expired\"\n      ],\n      \"example\": \"pending\"\n    },\n    \"checkout_flow_type\": {\n      \"type\": \"string\",\n      \"description\": \"The checkout flow type used for this session.\"\
  ,\n      \"example\": \"classic\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for the checkout.\",\n      \"example\": \"USD\"\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total checkout amount in cents.\",\n      \"example\": 1\n    },\n    \"shipping_amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Shipping cost in cents.\",\n      \"example\": 1\n    },\n    \"tax_amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Tax amount in cents.\",\n      \"example\": 1\n    },\n    \"order_id\": {\n      \"type\": \"string\",\n      \"description\": \"Merchant's internal order identifier.\",\n      \"example\": \"500123\"\n    },\n    \"financial_program_name\": {\n      \"type\": \"string\",\n      \"description\": \"Internal financing program identifier applied to this checkout.\",\n      \"example\": \"Example Merchant\"\n    },\n    \"financial_program_external_name\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Customer-facing financing program name.\",\n      \"example\": \"Example Merchant\"\n    },\n    \"billing_frequency\": {\n      \"type\": \"string\",\n      \"description\": \"Loan billing frequency for the financing applied.\",\n      \"example\": \"example_value\"\n    },\n    \"api_version\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the Affirm API used to create this checkout.\",\n      \"example\": \"example_value\"\n    },\n    \"product_type\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Product category associated with this checkout, if set.\",\n      \"example\": \"standard\"\n    },\n    \"billing\": {\n      \"$ref\": \"#/components/schemas/ContactObject\"\n    },\n    \"shipping\": {\n      \"$ref\": \"#/components/schemas/ContactObject\"\n    },\n    \"merchant\": {\n      \"$ref\": \"#/components/schemas/MerchantObject\"\n    },\n    \"metadata\":\
  \ {\n      \"type\": \"object\",\n      \"description\": \"Additional checkout metadata.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {}\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"description\": \"Affirm internal tracking information.\",\n      \"properties\": {\n        \"user_timezone\": {\n          \"type\": \"string\",\n          \"description\": \"The user's timezone at time of checkout.\"\n        },\n        \"tracking_uuid\": {\n          \"type\": \"string\",\n          \"description\": \"Internal tracking UUID for this checkout session.\"\n        }\n      },\n      \"example\": {\n        \"user_timezone\": \"2025-03-15T14:30:00Z\",\n        \"tracking_uuid\": \"550e8400-e29b-41d4-a716-446655440000\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-checkout-schema.json
tags: []
title: Checkout
---
