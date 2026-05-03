---
description: This object represents a customer of your business. Use it to create recurring charges and track payments that belong to the same customer.
layout: schema
name: Stripe Customer
properties_list:
- description: Unique identifier for the object.
  name: id
  type: string
- description: String representing the object's type.
  name: object
  type: string
- description: The customer's address.
  name: address
  type: object
- description: The current balance, if any, that's stored on the customer. Positive amounts represent the amount the customer owes; negative amounts represent credit.
  name: balance
  type: integer
- description: Time at which the object was created. Measured in seconds since the Unix epoch.
  name: created
  type: integer
- description: Three-letter ISO code for the currency the customer can be charged in for recurring billing purposes.
  name: currency
  type:
  - string
  - 'null'
- description: ID of the default payment source for the customer.
  name: default_source
  type:
  - string
  - 'null'
- description: Whether or not the latest charge for the customer's latest invoice has failed.
  name: delinquent
  type:
  - boolean
  - 'null'
- description: An arbitrary string attached to the object.
  name: description
  type:
  - string
  - 'null'
- description: Describes the current discount active on the customer, if there is one.
  name: discount
  type: object
- description: The customer's email address.
  name: email
  type:
  - string
  - 'null'
- description: The prefix for the customer used to generate unique invoice numbers.
  name: invoice_prefix
  type:
  - string
  - 'null'
- description: The customer's default invoice settings.
  name: invoice_settings
  type:
  - object
  - 'null'
- description: Has the value true if the object exists in live mode or the value false if the object exists in test mode.
  name: livemode
  type: boolean
- description: Set of key-value pairs that you can attach to an object.
  name: metadata
  type: object
- description: The customer's full name or business name.
  name: name
  type:
  - string
  - 'null'
- description: The suffix of the customer's next invoice number.
  name: next_invoice_sequence
  type: integer
- description: The customer's phone number.
  name: phone
  type:
  - string
  - 'null'
- description: The customer's preferred locales (languages), ordered by preference.
  name: preferred_locales
  type: array
- description: Mailing and shipping address for the customer.
  name: shipping
  type: object
- description: The customer's payment sources, if any.
  name: sources
  type: object
- description: The customer's current subscriptions, if any.
  name: subscriptions
  type: object
- description: Describes the customer's tax exemption status.
  name: tax_exempt
  type:
  - string
  - 'null'
- description: The customer's tax IDs.
  name: tax_ids
  type: object
- description: ID of the test clock that this customer belongs to.
  name: test_clock
  type:
  - string
  - 'null'
provider_name: Stripe
provider_slug: stripe
schema_file: json-schema/stripe-customer.json
slug: stripe-customer
source_filename: stripe-customer.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://stripe.com/schemas/customer\",\n  \"title\": \"Stripe Customer\",\n  \"description\": \"This object represents a customer of your business. Use it to create recurring charges and track payments that belong to the same customer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the object.\",\n      \"pattern\": \"^cus_\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"customer\",\n      \"description\": \"String representing the object's type.\"\n    },\n    \"address\": {\n      \"description\": \"The customer's address.\",\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/address\" },\n        { \"type\": \"null\" }\n      ]\n    },\n    \"balance\": {\n      \"type\": \"integer\",\n      \"description\": \"The current balance, if any, that's stored on the customer.\
  \ Positive amounts represent the amount the customer owes; negative amounts represent credit.\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Time at which the object was created. Measured in seconds since the Unix epoch.\"\n    },\n    \"currency\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Three-letter ISO code for the currency the customer can be charged in for recurring billing purposes.\"\n    },\n    \"default_source\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the default payment source for the customer.\"\n    },\n    \"delinquent\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Whether or not the latest charge for the customer's latest invoice has failed.\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An arbitrary string attached to the object.\"\n    },\n    \"discount\": {\n      \"description\": \"Describes\
  \ the current discount active on the customer, if there is one.\",\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/discount\" },\n        { \"type\": \"null\" }\n      ]\n    },\n    \"email\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The customer's email address.\",\n      \"format\": \"email\"\n    },\n    \"invoice_prefix\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The prefix for the customer used to generate unique invoice numbers.\"\n    },\n    \"invoice_settings\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The customer's default invoice settings.\",\n      \"properties\": {\n        \"custom_fields\": {\n          \"type\": [\"array\", \"null\"],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": { \"type\": \"string\" },\n              \"value\": { \"type\": \"string\" }\n            }\n          }\n        },\n        \"default_payment_method\"\
  : {\n          \"type\": [\"string\", \"null\"]\n        },\n        \"footer\": {\n          \"type\": [\"string\", \"null\"]\n        },\n        \"rendering_options\": {\n          \"type\": [\"object\", \"null\"]\n        }\n      }\n    },\n    \"livemode\": {\n      \"type\": \"boolean\",\n      \"description\": \"Has the value true if the object exists in live mode or the value false if the object exists in test mode.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Set of key-value pairs that you can attach to an object.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The customer's full name or business name.\"\n    },\n    \"next_invoice_sequence\": {\n      \"type\": \"integer\",\n      \"description\": \"The suffix of the customer's next invoice number.\"\n    },\n    \"phone\": {\n      \"type\": [\"string\", \"null\"\
  ],\n      \"description\": \"The customer's phone number.\"\n    },\n    \"preferred_locales\": {\n      \"type\": \"array\",\n      \"description\": \"The customer's preferred locales (languages), ordered by preference.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"shipping\": {\n      \"description\": \"Mailing and shipping address for the customer.\",\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/shipping\" },\n        { \"type\": \"null\" }\n      ]\n    },\n    \"sources\": {\n      \"type\": \"object\",\n      \"description\": \"The customer's payment sources, if any.\"\n    },\n    \"subscriptions\": {\n      \"type\": \"object\",\n      \"description\": \"The customer's current subscriptions, if any.\"\n    },\n    \"tax_exempt\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Describes the customer's tax exemption status.\",\n      \"enum\": [\"exempt\", \"none\", \"reverse\", null]\n    },\n    \"tax_ids\": {\n      \"\
  type\": \"object\",\n      \"description\": \"The customer's tax IDs.\"\n    },\n    \"test_clock\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the test clock that this customer belongs to.\"\n    }\n  },\n  \"required\": [\"id\", \"object\", \"created\", \"livemode\", \"metadata\"],\n  \"$defs\": {\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"city\": { \"type\": [\"string\", \"null\"] },\n        \"country\": { \"type\": [\"string\", \"null\"] },\n        \"line1\": { \"type\": [\"string\", \"null\"] },\n        \"line2\": { \"type\": [\"string\", \"null\"] },\n        \"postal_code\": { \"type\": [\"string\", \"null\"] },\n        \"state\": { \"type\": [\"string\", \"null\"] }\n      }\n    },\n    \"discount\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"object\": { \"type\": \"string\", \"const\": \"discount\" },\n        \"coupon\": { \"type\"\
  : \"object\" },\n        \"customer\": { \"type\": [\"string\", \"null\"] },\n        \"end\": { \"type\": [\"integer\", \"null\"] },\n        \"start\": { \"type\": \"integer\" },\n        \"subscription\": { \"type\": [\"string\", \"null\"] }\n      }\n    },\n    \"shipping\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"address\": { \"$ref\": \"#/$defs/address\" },\n        \"name\": { \"type\": \"string\" },\n        \"phone\": { \"type\": [\"string\", \"null\"] }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/stripe/refs/heads/main/json-schema/stripe-customer.json
tags:
- Commerce
- Financial Services
- Fintech
- Payments
- T1
title: Stripe Customer
---
