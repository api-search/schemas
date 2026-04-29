---
description: Represents a payment processed by Square.
layout: schema
name: Payment
properties_list:
- description: Unique ID for this payment.
  name: id
  type: string
- description: Indicates whether the payment is APPROVED, COMPLETED, CANCELED, or FAILED.
  name: status
  type: string
- description: The source type for this payment.
  name: source_type
  type: string
- description: ''
  name: amount_money
  type: object
- description: ''
  name: total_money
  type: object
- description: The ID of the location associated with the payment.
  name: location_id
  type: string
- description: The timestamp of when the payment was created.
  name: created_at
  type: string
- description: The timestamp of when the payment was last updated.
  name: updated_at
  type: string
provider_name: Block
provider_slug: block
schema_file: json-schema/block-payment-schema.json
slug: block-payment
source_filename: block-payment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/block/main/json-schema/block-payment-schema.json\",\n  \"title\": \"Payment\",\n  \"description\": \"Represents a payment processed by Square.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID for this payment.\",\n      \"example\": \"GQTFp1ZlXdpoW4o6eGiZhbjosiDFf\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates whether the payment is APPROVED, COMPLETED, CANCELED, or FAILED.\",\n      \"enum\": [\"APPROVED\", \"COMPLETED\", \"CANCELED\", \"FAILED\"],\n      \"example\": \"COMPLETED\"\n    },\n    \"source_type\": {\n      \"type\": \"string\",\n      \"description\": \"The source type for this payment.\",\n      \"example\": \"CARD\"\n    },\n    \"amount_money\": {\n      \"$ref\": \"#/$defs/Money\"\n    },\n    \"total_money\"\
  : {\n      \"$ref\": \"#/$defs/Money\"\n    },\n    \"location_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the location associated with the payment.\",\n      \"example\": \"L1234567890\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp of when the payment was created.\",\n      \"example\": \"2026-01-15T10:00:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp of when the payment was last updated.\",\n      \"example\": \"2026-01-15T10:00:05Z\"\n    }\n  },\n  \"$defs\": {\n    \"Money\": {\n      \"type\": \"object\",\n      \"description\": \"Represents an amount of money in a specific currency.\",\n      \"properties\": {\n        \"amount\": {\n          \"type\": \"integer\",\n          \"description\": \"Amount in the smallest denomination of the currency.\",\n          \"example\"\
  : 1500\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"3-letter ISO 4217 currency code.\",\n          \"example\": \"USD\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/block/refs/heads/main/json-schema/block-payment-schema.json
tags:
- Commerce
- Cryptocurrency
- eCommerce
- Fintech
- Payments
- Point Of Sale
- Square
title: Payment
---
