---
description: Represents an Affirm-issued virtual card number (VCN) used in the Affirm Lite integration pattern to process payments through traditional card networks.
layout: schema
name: Card
properties_list:
- description: Unique identifier for this virtual card.
  name: id
  type: string
- description: Checkout session identifier associated with this card.
  name: checkout_id
  type: string
- description: Current status of the virtual card.
  name: status
  type: string
- description: Virtual card number (PAN).
  name: number
  type: string
- description: Card verification value.
  name: cvv
  type: string
- description: Card expiration date in MM/YY format.
  name: expiration
  type: string
- description: Billing address associated with this virtual card.
  name: billing
  type: object
- description: Authorized amount on this virtual card in cents.
  name: amount
  type: integer
- description: ISO 4217 currency code.
  name: currency
  type: string
- description: Card creation timestamp in RFC 3339 format.
  name: created
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/direct-api-card-schema.json
slug: direct-api-card
source_filename: direct-api-card-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/direct-api-card-schema.json\",\n  \"title\": \"Card\",\n  \"description\": \"Represents an Affirm-issued virtual card number (VCN) used in the Affirm Lite integration pattern to process payments through traditional card networks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this virtual card.\",\n      \"example\": \"500123\"\n    },\n    \"checkout_id\": {\n      \"type\": \"string\",\n      \"description\": \"Checkout session identifier associated with this card.\",\n      \"example\": \"500123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the virtual card.\",\n      \"enum\": [\n        \"active\",\n        \"cancelled\",\n        \"finalized\"\n      ],\n  \
  \    \"example\": \"active\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Virtual card number (PAN).\",\n      \"example\": \"example_value\"\n    },\n    \"cvv\": {\n      \"type\": \"string\",\n      \"description\": \"Card verification value.\",\n      \"example\": \"example_value\"\n    },\n    \"expiration\": {\n      \"type\": \"string\",\n      \"description\": \"Card expiration date in MM/YY format.\",\n      \"example\": \"example_value\"\n    },\n    \"billing\": {\n      \"type\": \"object\",\n      \"description\": \"Billing address associated with this virtual card.\",\n      \"properties\": {\n        \"address\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"line1\": {\n              \"type\": \"string\",\n              \"description\": \"Street address line 1.\"\n            },\n            \"city\": {\n              \"type\": \"string\",\n              \"description\": \"City.\"\n            },\n   \
  \         \"state\": {\n              \"type\": \"string\",\n              \"description\": \"State code.\"\n            },\n            \"zipcode\": {\n              \"type\": \"string\",\n              \"description\": \"ZIP or postal code.\"\n            },\n            \"country\": {\n              \"type\": \"string\",\n              \"description\": \"ISO 3166-1 alpha-2 country code.\"\n            }\n          }\n        }\n      },\n      \"example\": {\n        \"address\": {\n          \"line1\": \"example_value\",\n          \"city\": \"example_value\",\n          \"state\": \"example_value\",\n          \"zipcode\": \"example_value\",\n          \"country\": \"example_value\"\n        }\n      }\n    },\n    \"amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Authorized amount on this virtual card in cents.\",\n      \"example\": 1\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code.\",\n      \"example\"\
  : \"USD\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Card creation timestamp in RFC 3339 format.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/direct-api-card-schema.json
tags: []
title: Card
---
