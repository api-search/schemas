---
description: Request body for creating or updating an Affirm checkout session, containing all order and customer information required to initiate the Affirm financing flow.
layout: schema
name: CheckoutRequest
properties_list:
- description: ''
  name: merchant
  type: object
- description: ''
  name: shipping
  type: object
- description: ''
  name: billing
  type: object
- description: ''
  name: store
  type: object
- description: Array of item objects representing the products being purchased in this checkout.
  name: items
  type: array
- description: A map of discount codes to discount objects. Each key is the discount code and each value contains the discount amount and name.
  name: discounts
  type: object
- description: Arbitrary key-value metadata for merchant tracking. Values must be strings.
  name: metadata
  type: object
- description: The merchant's internal order identifier. Stored for future reference and reconciliation.
  name: order_id
  type: string
- description: Three-letter ISO 4217 currency code in uppercase. Supported values are USD, CAD, and GBP.
  name: currency
  type: string
- description: Financing program code to apply to this checkout, if applicable. Determines the available loan terms presented to the customer.
  name: financing_program
  type: string
- description: The total shipping amount in cents.
  name: shipping_amount
  type: integer
- description: The total tax amount in cents.
  name: tax_amount
  type: integer
- description: The total amount of the checkout in cents (USD, CAD) or pence (GBP).
  name: total
  type: integer
- description: ISO 8601 timestamp specifying when the checkout session expires.
  name: checkout_expiration
  type: string
- description: Time-to-live deadline by which the customer must confirm the checkout.
  name: expiration_time
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/checkout-checkout-request-schema.json
slug: checkout-checkout-request
source_filename: checkout-checkout-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-checkout-request-schema.json\",\n  \"title\": \"CheckoutRequest\",\n  \"description\": \"Request body for creating or updating an Affirm checkout session, containing all order and customer information required to initiate the Affirm financing flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchant\": {\n      \"$ref\": \"#/components/schemas/MerchantObject\"\n    },\n    \"shipping\": {\n      \"$ref\": \"#/components/schemas/ContactObject\"\n    },\n    \"billing\": {\n      \"$ref\": \"#/components/schemas/ContactObject\"\n    },\n    \"store\": {\n      \"$ref\": \"#/components/schemas/StoreObject\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Array of item objects representing the products being purchased in this checkout.\",\n      \"items\": {\n \
  \       \"$ref\": \"#/components/schemas/ItemObject\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"discounts\": {\n      \"type\": \"object\",\n      \"description\": \"A map of discount codes to discount objects. Each key is the discount code and each value contains the discount amount and name.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/DiscountObject\"\n      },\n      \"example\": {}\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Arbitrary key-value metadata for merchant tracking. Values must be strings.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {}\n    },\n    \"order_id\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant's internal order identifier. Stored for future reference and reconciliation.\",\n      \"example\": \"500123\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"Three-letter ISO 4217 currency code in uppercase. Supported values are USD, CAD, and GBP.\",\n      \"enum\": [\n        \"USD\",\n        \"CAD\",\n        \"GBP\"\n      ],\n      \"example\": \"USD\"\n    },\n    \"financing_program\": {\n      \"type\": \"string\",\n      \"description\": \"Financing program code to apply to this checkout, if applicable. Determines the available loan terms presented to the customer.\",\n      \"example\": \"example_value\"\n    },\n    \"shipping_amount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total shipping amount in cents.\",\n      \"minimum\": 0,\n      \"example\": 1\n    },\n    \"tax_amount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total tax amount in cents.\",\n      \"minimum\": 0,\n      \"example\": 1\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"The total amount of the checkout in cents (USD, CAD) or pence (GBP).\",\n      \"minimum\"\
  : 0,\n      \"example\": 1\n    },\n    \"checkout_expiration\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp specifying when the checkout session expires.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"expiration_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time-to-live deadline by which the customer must confirm the checkout.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"required\": [\n    \"merchant\",\n    \"items\",\n    \"currency\",\n    \"total\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-checkout-request-schema.json
tags: []
title: CheckoutRequest
---
