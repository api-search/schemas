---
description: Represents an amount of money. Money fields can be signed or unsigned. The amount is specified in the smallest denomination of the applicable currency (for example, US dollar amounts are specified in cents).
layout: schema
name: Square Money
properties_list:
- description: The amount of money, in the smallest denomination of the currency indicated by currency. For example, when currency is USD, amount is in cents.
  name: amount
  type: integer
- description: The type of currency, in ISO 4217 format. For example, the currency code for US dollars is USD.
  name: currency
  type: string
provider_name: Square
provider_slug: square
schema_file: json-schema/money.json
slug: money
source_json: "{\n  \"$id\": \"https://github.com/api-evangelist/square/blob/main/json-schema/money.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Square Money\",\n  \"description\": \"Represents an amount of money. Money fields can be signed or unsigned. The amount is specified in the smallest denomination of the applicable currency (for example, US dollar amounts are specified in cents).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The amount of money, in the smallest denomination of the currency indicated by currency. For example, when currency is USD, amount is in cents.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The type of currency, in ISO 4217 format. For example, the currency code for US dollars is USD.\",\n      \"minLength\": 3,\n      \"maxLength\": 3\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/square/refs/heads/main/json-schema/money.json
tags:
- Bookings
- Catalog
- Checkout
- Customers
- Disputes
- Ecommerce
- Financial Technology
- Gift Cards
- Inventory
- Invoicing
- Labor
- Locations
- Loyalty
- Merchants
- Orders
- Payments
- Point of Sale
- Refunds
- Retail
- Subscriptions
- Team
- Terminal
- Webhooks
title: Square Money
---
