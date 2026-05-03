---
description: A gift card order placed through the Reloadly Gift Cards API
layout: schema
name: Reloadly Gift Card Order
properties_list:
- description: Unique transaction identifier
  name: transactionId
  type: integer
- description: Amount charged for the order
  name: amount
  type: number
- description: Discount amount applied
  name: discount
  type: number
- description: ISO 4217 currency code for the transaction
  name: currencyCode
  type: string
- description: Processing fee charged
  name: fee
  type: number
- description: Email address of the gift card recipient
  name: recipientEmail
  type: string
- description: Custom reference identifier provided at order time
  name: customIdentifier
  type: string
- description: Order fulfillment status
  name: status
  type: string
- description: The ordered gift card product
  name: product
  type: object
- description: Gift card codes delivered in this order
  name: smiles
  type: array
- description: Order placement timestamp
  name: date
  type: string
provider_name: Reloadly
provider_slug: reloadly
schema_file: json-schema/reloadly-order-schema.json
slug: reloadly-order
source_filename: reloadly-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://api-evangelist.github.io/reloadly/json-schema/reloadly-order-schema.json\",\n  \"title\": \"Reloadly Gift Card Order\",\n  \"description\": \"A gift card order placed through the Reloadly Gift Cards API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique transaction identifier\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Amount charged for the order\"\n    },\n    \"discount\": {\n      \"type\": \"number\",\n      \"description\": \"Discount amount applied\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"ISO 4217 currency code for the transaction\"\n    },\n    \"fee\": {\n      \"type\": \"number\",\n      \"description\": \"Processing fee charged\"\n    },\n    \"recipientEmail\": {\n      \"\
  type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the gift card recipient\"\n    },\n    \"customIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"Custom reference identifier provided at order time\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Order fulfillment status\"\n    },\n    \"product\": {\n      \"$ref\": \"reloadly-product-schema.json\",\n      \"description\": \"The ordered gift card product\"\n    },\n    \"smiles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/GiftCard\"\n      },\n      \"description\": \"Gift card codes delivered in this order\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Order placement timestamp\"\n    }\n  },\n  \"required\": [\"transactionId\", \"status\"],\n  \"$defs\": {\n    \"GiftCard\": {\n      \"type\": \"object\",\n      \"description\": \"\
  A delivered digital gift card\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Gift card redemption code\"\n        },\n        \"pinCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"PIN code required for redemption (if applicable)\"\n        },\n        \"validity\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Expiration date or validity period\"\n        }\n      },\n      \"required\": [\"code\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/json-schema/reloadly-order-schema.json
tags:
- Gift Cards
- Payments
- Airtime
- Mobile Top-Up
- Rewards
- Incentives
title: Reloadly Gift Card Order
---
