---
description: Prices define the unit cost, currency, and (optional) billing cycle for both recurring and one-time purchases of products.
layout: schema
name: Stripe Price
properties_list:
- description: Unique identifier for the object.
  name: id
  type: string
- description: String representing the object's type.
  name: object
  type: string
- description: Whether the price can be used for new purchases.
  name: active
  type: boolean
- description: Describes how to compute the price per period.
  name: billing_scheme
  type: string
- description: Time at which the object was created.
  name: created
  type: integer
- description: Three-letter ISO currency code, in lowercase.
  name: currency
  type: string
- description: Prices defined in each available currency option.
  name: currency_options
  type:
  - object
  - 'null'
- description: When set, provides configuration for the amount to be adjusted by the customer during Checkout Sessions and Payment Links.
  name: custom_unit_amount
  type:
  - object
  - 'null'
- description: Has the value true if the object exists in live mode.
  name: livemode
  type: boolean
- description: A lookup key used to retrieve prices dynamically from a static string.
  name: lookup_key
  type:
  - string
  - 'null'
- description: Set of key-value pairs that you can attach to an object.
  name: metadata
  type: object
- description: A brief description of the price, hidden from customers.
  name: nickname
  type:
  - string
  - 'null'
- description: The ID of the product this price is associated with.
  name: product
  type: string
- description: The recurring components of a price such as interval and usage_type.
  name: recurring
  type:
  - object
  - 'null'
- description: Only required for products with multiple prices.
  name: tax_behavior
  type:
  - string
  - 'null'
- description: Each element represents a pricing tier.
  name: tiers
  type:
  - array
  - 'null'
- description: Defines if the tiering price should be graduated or volume based.
  name: tiers_mode
  type:
  - string
  - 'null'
- description: Apply a transformation to the reported usage or set quantity before computing the amount billed.
  name: transform_quantity
  type:
  - object
  - 'null'
- description: One of one_time or recurring depending on whether the price is for a one-time purchase or a recurring (subscription) purchase.
  name: type
  type: string
- description: The unit amount in cents to be charged.
  name: unit_amount
  type:
  - integer
  - 'null'
- description: The unit amount in cents to be charged, represented as a decimal string with at most 12 decimal places.
  name: unit_amount_decimal
  type:
  - string
  - 'null'
provider_name: Stripe
provider_slug: stripe
schema_file: json-schema/stripe-price.json
slug: stripe-price
source_filename: stripe-price.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://stripe.com/schemas/price\",\n  \"title\": \"Stripe Price\",\n  \"description\": \"Prices define the unit cost, currency, and (optional) billing cycle for both recurring and one-time purchases of products.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the object.\",\n      \"pattern\": \"^price_\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"price\",\n      \"description\": \"String representing the object's type.\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the price can be used for new purchases.\"\n    },\n    \"billing_scheme\": {\n      \"type\": \"string\",\n      \"description\": \"Describes how to compute the price per period.\",\n      \"enum\": [\"per_unit\", \"tiered\"]\n    },\n    \"created\": {\n     \
  \ \"type\": \"integer\",\n      \"description\": \"Time at which the object was created.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Three-letter ISO currency code, in lowercase.\"\n    },\n    \"currency_options\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Prices defined in each available currency option.\"\n    },\n    \"custom_unit_amount\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"When set, provides configuration for the amount to be adjusted by the customer during Checkout Sessions and Payment Links.\",\n      \"properties\": {\n        \"maximum\": { \"type\": [\"integer\", \"null\"] },\n        \"minimum\": { \"type\": [\"integer\", \"null\"] },\n        \"preset\": { \"type\": [\"integer\", \"null\"] }\n      }\n    },\n    \"livemode\": {\n      \"type\": \"boolean\",\n      \"description\": \"Has the value true if the object exists in live mode.\"\n    },\n    \"lookup_key\": {\n\
  \      \"type\": [\"string\", \"null\"],\n      \"description\": \"A lookup key used to retrieve prices dynamically from a static string.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Set of key-value pairs that you can attach to an object.\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"nickname\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A brief description of the price, hidden from customers.\"\n    },\n    \"product\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the product this price is associated with.\"\n    },\n    \"recurring\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The recurring components of a price such as interval and usage_type.\",\n      \"properties\": {\n        \"aggregate_usage\": {\n          \"type\": [\"string\", \"null\"],\n          \"enum\": [\"last_during_period\", \"last_ever\", \"max\", \"sum\", null]\n       \
  \ },\n        \"interval\": {\n          \"type\": \"string\",\n          \"enum\": [\"day\", \"month\", \"week\", \"year\"]\n        },\n        \"interval_count\": {\n          \"type\": \"integer\"\n        },\n        \"trial_period_days\": {\n          \"type\": [\"integer\", \"null\"]\n        },\n        \"usage_type\": {\n          \"type\": \"string\",\n          \"enum\": [\"licensed\", \"metered\"]\n        }\n      },\n      \"required\": [\"interval\", \"interval_count\", \"usage_type\"]\n    },\n    \"tax_behavior\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Only required for products with multiple prices.\",\n      \"enum\": [\"exclusive\", \"inclusive\", \"unspecified\", null]\n    },\n    \"tiers\": {\n      \"type\": [\"array\", \"null\"],\n      \"description\": \"Each element represents a pricing tier.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"flat_amount\": { \"type\": [\"integer\", \"null\"\
  ] },\n          \"flat_amount_decimal\": { \"type\": [\"string\", \"null\"] },\n          \"unit_amount\": { \"type\": [\"integer\", \"null\"] },\n          \"unit_amount_decimal\": { \"type\": [\"string\", \"null\"] },\n          \"up_to\": { \"type\": [\"integer\", \"null\"] }\n        }\n      }\n    },\n    \"tiers_mode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Defines if the tiering price should be graduated or volume based.\",\n      \"enum\": [\"graduated\", \"volume\", null]\n    },\n    \"transform_quantity\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Apply a transformation to the reported usage or set quantity before computing the amount billed.\",\n      \"properties\": {\n        \"divide_by\": { \"type\": \"integer\" },\n        \"round\": { \"type\": \"string\", \"enum\": [\"down\", \"up\"] }\n      }\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"One of one_time or recurring depending\
  \ on whether the price is for a one-time purchase or a recurring (subscription) purchase.\",\n      \"enum\": [\"one_time\", \"recurring\"]\n    },\n    \"unit_amount\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The unit amount in cents to be charged.\"\n    },\n    \"unit_amount_decimal\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The unit amount in cents to be charged, represented as a decimal string with at most 12 decimal places.\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"object\",\n    \"active\",\n    \"billing_scheme\",\n    \"created\",\n    \"currency\",\n    \"livemode\",\n    \"metadata\",\n    \"product\",\n    \"type\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/stripe/refs/heads/main/json-schema/stripe-price.json
tags:
- Commerce
- Financial Services
- Fintech
- Payments
- T1
title: Stripe Price
---
