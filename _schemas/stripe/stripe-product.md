---
description: Products describe the specific goods or services you offer to your customers. They can be used in conjunction with Prices to configure pricing in Payment Links, Checkout, and Subscriptions.
layout: schema
name: Stripe Product
properties_list:
- description: Unique identifier for the object.
  name: id
  type: string
- description: String representing the object's type.
  name: object
  type: string
- description: Whether the product is currently available for purchase.
  name: active
  type: boolean
- description: Time at which the object was created.
  name: created
  type: integer
- description: The ID of the Price object that is the default price for this product.
  name: default_price
  type:
  - string
  - 'null'
- description: The product's description, meant to be displayable to the customer.
  name: description
  type:
  - string
  - 'null'
- description: A list of up to 15 features for this product.
  name: features
  type: array
- description: A list of up to 8 URLs of images for this product.
  name: images
  type: array
- description: Has the value true if the object exists in live mode.
  name: livemode
  type: boolean
- description: Set of key-value pairs that you can attach to an object.
  name: metadata
  type: object
- description: The product's name, meant to be displayable to the customer.
  name: name
  type: string
- description: The dimensions of this product for shipping purposes.
  name: package_dimensions
  type:
  - object
  - 'null'
- description: Whether this product is shipped (i.e., physical goods).
  name: shippable
  type:
  - boolean
  - 'null'
- description: Extra information about a product which will appear on your customer's credit card statement.
  name: statement_descriptor
  type:
  - string
  - 'null'
- description: A tax code ID.
  name: tax_code
  type:
  - string
  - 'null'
- description: The type of the product.
  name: type
  type: string
- description: A label that represents units of this product.
  name: unit_label
  type:
  - string
  - 'null'
- description: Time at which the object was last updated.
  name: updated
  type: integer
- description: A URL of a publicly-accessible webpage for this product.
  name: url
  type:
  - string
  - 'null'
provider_name: Stripe
provider_slug: stripe
schema_file: json-schema/stripe-product.json
slug: stripe-product
source_filename: stripe-product.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://stripe.com/schemas/product\",\n  \"title\": \"Stripe Product\",\n  \"description\": \"Products describe the specific goods or services you offer to your customers. They can be used in conjunction with Prices to configure pricing in Payment Links, Checkout, and Subscriptions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the object.\",\n      \"pattern\": \"^prod_\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"product\",\n      \"description\": \"String representing the object's type.\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the product is currently available for purchase.\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Time at which the object was created.\"\n    },\n    \"\
  default_price\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the Price object that is the default price for this product.\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The product's description, meant to be displayable to the customer.\"\n    },\n    \"features\": {\n      \"type\": \"array\",\n      \"description\": \"A list of up to 15 features for this product.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": { \"type\": \"string\" }\n        },\n        \"required\": [\"name\"]\n      }\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"description\": \"A list of up to 8 URLs of images for this product.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      }\n    },\n    \"livemode\": {\n      \"type\": \"boolean\",\n      \"description\": \"Has the value true if the object exists in live mode.\"\
  \n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Set of key-value pairs that you can attach to an object.\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The product's name, meant to be displayable to the customer.\"\n    },\n    \"package_dimensions\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The dimensions of this product for shipping purposes.\",\n      \"properties\": {\n        \"height\": { \"type\": \"number\" },\n        \"length\": { \"type\": \"number\" },\n        \"weight\": { \"type\": \"number\" },\n        \"width\": { \"type\": \"number\" }\n      }\n    },\n    \"shippable\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Whether this product is shipped (i.e., physical goods).\"\n    },\n    \"statement_descriptor\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Extra information\
  \ about a product which will appear on your customer's credit card statement.\"\n    },\n    \"tax_code\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A tax code ID.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the product.\",\n      \"enum\": [\"good\", \"service\"]\n    },\n    \"unit_label\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A label that represents units of this product.\"\n    },\n    \"updated\": {\n      \"type\": \"integer\",\n      \"description\": \"Time at which the object was last updated.\"\n    },\n    \"url\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A URL of a publicly-accessible webpage for this product.\",\n      \"format\": \"uri\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"object\",\n    \"active\",\n    \"created\",\n    \"features\",\n    \"images\",\n    \"livemode\",\n    \"metadata\",\n    \"name\",\n    \"type\",\n \
  \   \"updated\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/stripe/refs/heads/main/json-schema/stripe-product.json
tags:
- Commerce
- Financial Services
- Fintech
- Payments
- T1
title: Stripe Product
---
