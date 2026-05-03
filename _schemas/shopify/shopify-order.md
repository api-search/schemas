---
description: An order placed in a Shopify store. Orders are records of purchases made by customers, including line items, payment status, fulfillment status, shipping, and billing information.
layout: schema
name: Shopify Order
properties_list:
- description: Unique numeric identifier for the order
  name: id
  type: integer
- description: 'The order name as displayed to the merchant (e.g. #1001)'
  name: name
  type: string
- description: The order sequential number without the prefix
  name: order_number
  type: integer
- description: The customer email address
  name: email
  type:
  - string
  - 'null'
- description: The customer phone number
  name: phone
  type:
  - string
  - 'null'
- description: When the order was created
  name: created_at
  type: string
- description: When the order was last updated
  name: updated_at
  type: string
- description: When the order was closed
  name: closed_at
  type:
  - string
  - 'null'
- description: When the order was cancelled
  name: cancelled_at
  type:
  - string
  - 'null'
- description: The reason for cancellation
  name: cancel_reason
  type:
  - string
  - 'null'
- description: Notes about the order
  name: note
  type:
  - string
  - 'null'
- description: Comma-separated tags
  name: tags
  type: string
- description: Unique token for the order
  name: token
  type: string
- description: The total price of the order including tax and shipping
  name: total_price
  type: string
- description: The subtotal price before shipping and taxes
  name: subtotal_price
  type: string
- description: The total tax amount
  name: total_tax
  type: string
- description: The total discount amount applied
  name: total_discounts
  type: string
- description: The total weight of all line items in grams
  name: total_weight
  type: integer
- description: The three-letter ISO 4217 currency code
  name: currency
  type: string
- description: The payment status of the order
  name: financial_status
  type: string
- description: The fulfillment status of the order
  name: fulfillment_status
  type:
  - string
  - 'null'
- description: Whether the order has been confirmed
  name: confirmed
  type: boolean
- description: Whether this is a test order
  name: test
  type: boolean
- description: Whether taxes are included in the order total
  name: taxes_included
  type: boolean
- description: Whether the buyer accepted marketing
  name: buyer_accepts_marketing
  type: boolean
- description: The total shipping price in shop and presentment currencies
  name: total_shipping_price_set
  type: object
- description: The customer who placed the order
  name: customer
  type: object
- description: ''
  name: billing_address
  type: object
- description: ''
  name: shipping_address
  type: object
- description: The line items in the order
  name: line_items
  type: array
- description: The shipping methods applied to the order
  name: shipping_lines
  type: array
- description: Tax lines applied to the order
  name: tax_lines
  type: array
- description: Discount codes applied to the order
  name: discount_codes
  type: array
- description: Fulfillments associated with the order
  name: fulfillments
  type: array
- description: Refunds associated with the order
  name: refunds
  type: array
- description: The GraphQL Admin API identifier
  name: admin_graphql_api_id
  type: string
provider_name: Shopify
provider_slug: shopify
schema_file: json-schema/shopify-order-schema.json
slug: shopify-order
source_filename: shopify-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://shopify.dev/schemas/order.json\",\n  \"title\": \"Shopify Order\",\n  \"description\": \"An order placed in a Shopify store. Orders are records of purchases made by customers, including line items, payment status, fulfillment status, shipping, and billing information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for the order\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The order name as displayed to the merchant (e.g. #1001)\"\n    },\n    \"order_number\": {\n      \"type\": \"integer\",\n      \"description\": \"The order sequential number without the prefix\"\n    },\n    \"email\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"email\",\n      \"description\": \"The customer email address\"\n    },\n    \"phone\": {\n      \"type\"\
  : [\"string\", \"null\"],\n      \"description\": \"The customer phone number\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the order was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the order was last updated\"\n    },\n    \"closed_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"When the order was closed\"\n    },\n    \"cancelled_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"When the order was cancelled\"\n    },\n    \"cancel_reason\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The reason for cancellation\",\n      \"enum\": [\"customer\", \"fraud\", \"inventory\", \"declined\", \"other\", null]\n    },\n    \"note\": {\n      \"type\": [\"string\", \"null\"],\n    \
  \  \"description\": \"Notes about the order\"\n    },\n    \"tags\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated tags\"\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"Unique token for the order\"\n    },\n    \"total_price\": {\n      \"type\": \"string\",\n      \"description\": \"The total price of the order including tax and shipping\"\n    },\n    \"subtotal_price\": {\n      \"type\": \"string\",\n      \"description\": \"The subtotal price before shipping and taxes\"\n    },\n    \"total_tax\": {\n      \"type\": \"string\",\n      \"description\": \"The total tax amount\"\n    },\n    \"total_discounts\": {\n      \"type\": \"string\",\n      \"description\": \"The total discount amount applied\"\n    },\n    \"total_weight\": {\n      \"type\": \"integer\",\n      \"description\": \"The total weight of all line items in grams\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The three-letter\
  \ ISO 4217 currency code\"\n    },\n    \"financial_status\": {\n      \"type\": \"string\",\n      \"description\": \"The payment status of the order\",\n      \"enum\": [\"pending\", \"authorized\", \"partially_paid\", \"paid\", \"partially_refunded\", \"refunded\", \"voided\"]\n    },\n    \"fulfillment_status\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The fulfillment status of the order\",\n      \"enum\": [\"fulfilled\", \"partial\", \"restocked\", null]\n    },\n    \"confirmed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the order has been confirmed\"\n    },\n    \"test\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a test order\"\n    },\n    \"taxes_included\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether taxes are included in the order total\"\n    },\n    \"buyer_accepts_marketing\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the buyer accepted marketing\"\
  \n    },\n    \"total_shipping_price_set\": {\n      \"type\": \"object\",\n      \"description\": \"The total shipping price in shop and presentment currencies\",\n      \"properties\": {\n        \"shop_money\": {\n          \"$ref\": \"#/$defs/Money\"\n        },\n        \"presentment_money\": {\n          \"$ref\": \"#/$defs/Money\"\n        }\n      }\n    },\n    \"customer\": {\n      \"type\": \"object\",\n      \"description\": \"The customer who placed the order\",\n      \"properties\": {\n        \"id\": { \"type\": \"integer\" },\n        \"email\": { \"type\": [\"string\", \"null\"] },\n        \"first_name\": { \"type\": [\"string\", \"null\"] },\n        \"last_name\": { \"type\": [\"string\", \"null\"] }\n      }\n    },\n    \"billing_address\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"shipping_address\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"line_items\": {\n      \"type\": \"array\",\n      \"description\": \"The line items in the order\"\
  ,\n      \"items\": {\n        \"$ref\": \"#/$defs/LineItem\"\n      }\n    },\n    \"shipping_lines\": {\n      \"type\": \"array\",\n      \"description\": \"The shipping methods applied to the order\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ShippingLine\"\n      }\n    },\n    \"tax_lines\": {\n      \"type\": \"array\",\n      \"description\": \"Tax lines applied to the order\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TaxLine\"\n      }\n    },\n    \"discount_codes\": {\n      \"type\": \"array\",\n      \"description\": \"Discount codes applied to the order\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"code\": { \"type\": \"string\" },\n          \"amount\": { \"type\": \"string\" },\n          \"type\": { \"type\": \"string\", \"enum\": [\"fixed_amount\", \"percentage\", \"shipping\"] }\n        }\n      }\n    },\n    \"fulfillments\": {\n      \"type\": \"array\",\n      \"description\": \"Fulfillments associated\
  \ with the order\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Fulfillment\"\n      }\n    },\n    \"refunds\": {\n      \"type\": \"array\",\n      \"description\": \"Refunds associated with the order\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Refund\"\n      }\n    },\n    \"admin_graphql_api_id\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL Admin API identifier\"\n    }\n  },\n  \"required\": [\"id\", \"name\"],\n  \"$defs\": {\n    \"LineItem\": {\n      \"type\": \"object\",\n      \"description\": \"An individual line item in an order\",\n      \"properties\": {\n        \"id\": { \"type\": \"integer\" },\n        \"variant_id\": { \"type\": [\"integer\", \"null\"] },\n        \"product_id\": { \"type\": [\"integer\", \"null\"] },\n        \"title\": { \"type\": \"string\" },\n        \"variant_title\": { \"type\": [\"string\", \"null\"] },\n        \"name\": { \"type\": \"string\", \"description\": \"Product title and variant title\" },\n\
  \        \"quantity\": { \"type\": \"integer\" },\n        \"price\": { \"type\": \"string\" },\n        \"total_discount\": { \"type\": \"string\" },\n        \"sku\": { \"type\": [\"string\", \"null\"] },\n        \"vendor\": { \"type\": [\"string\", \"null\"] },\n        \"fulfillment_service\": { \"type\": \"string\" },\n        \"fulfillment_status\": { \"type\": [\"string\", \"null\"] },\n        \"taxable\": { \"type\": \"boolean\" },\n        \"requires_shipping\": { \"type\": \"boolean\" },\n        \"gift_card\": { \"type\": \"boolean\" },\n        \"grams\": { \"type\": \"integer\" },\n        \"tax_lines\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/TaxLine\" }\n        },\n        \"properties\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": { \"type\": \"string\" },\n              \"value\": { \"type\": \"string\" }\n            }\n   \
  \       }\n        },\n        \"admin_graphql_api_id\": { \"type\": \"string\" }\n      },\n      \"required\": [\"id\", \"title\", \"quantity\", \"price\"]\n    },\n    \"ShippingLine\": {\n      \"type\": \"object\",\n      \"description\": \"A shipping method applied to the order\",\n      \"properties\": {\n        \"id\": { \"type\": \"integer\" },\n        \"title\": { \"type\": \"string\" },\n        \"price\": { \"type\": \"string\" },\n        \"code\": { \"type\": [\"string\", \"null\"] },\n        \"source\": { \"type\": \"string\" },\n        \"discounted_price\": { \"type\": \"string\" },\n        \"tax_lines\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/TaxLine\" }\n        }\n      }\n    },\n    \"TaxLine\": {\n      \"type\": \"object\",\n      \"description\": \"A tax line\",\n      \"properties\": {\n        \"title\": { \"type\": \"string\" },\n        \"price\": { \"type\": \"string\" },\n        \"rate\": { \"type\": \"number\"\
  \ }\n      }\n    },\n    \"Money\": {\n      \"type\": \"object\",\n      \"description\": \"A monetary amount with currency\",\n      \"properties\": {\n        \"amount\": { \"type\": \"string\" },\n        \"currency_code\": { \"type\": \"string\" }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A mailing address\",\n      \"properties\": {\n        \"first_name\": { \"type\": [\"string\", \"null\"] },\n        \"last_name\": { \"type\": [\"string\", \"null\"] },\n        \"company\": { \"type\": [\"string\", \"null\"] },\n        \"address1\": { \"type\": [\"string\", \"null\"] },\n        \"address2\": { \"type\": [\"string\", \"null\"] },\n        \"city\": { \"type\": [\"string\", \"null\"] },\n        \"province\": { \"type\": [\"string\", \"null\"] },\n        \"country\": { \"type\": [\"string\", \"null\"] },\n        \"zip\": { \"type\": [\"string\", \"null\"] },\n        \"phone\": { \"type\": [\"string\", \"null\"] },\n       \
  \ \"province_code\": { \"type\": [\"string\", \"null\"] },\n        \"country_code\": { \"type\": [\"string\", \"null\"] },\n        \"latitude\": { \"type\": [\"number\", \"null\"] },\n        \"longitude\": { \"type\": [\"number\", \"null\"] }\n      }\n    },\n    \"Fulfillment\": {\n      \"type\": \"object\",\n      \"description\": \"A fulfillment of an order\",\n      \"properties\": {\n        \"id\": { \"type\": \"integer\" },\n        \"order_id\": { \"type\": \"integer\" },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"pending\", \"open\", \"success\", \"cancelled\", \"error\", \"failure\"]\n        },\n        \"tracking_company\": { \"type\": [\"string\", \"null\"] },\n        \"tracking_number\": { \"type\": [\"string\", \"null\"] },\n        \"tracking_numbers\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        },\n        \"tracking_url\": { \"type\": [\"string\", \"null\"] },\n        \"tracking_urls\"\
  : {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        },\n        \"created_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"updated_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"line_items\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/LineItem\" }\n        },\n        \"admin_graphql_api_id\": { \"type\": \"string\" }\n      }\n    },\n    \"Refund\": {\n      \"type\": \"object\",\n      \"description\": \"A refund on an order\",\n      \"properties\": {\n        \"id\": { \"type\": \"integer\" },\n        \"order_id\": { \"type\": \"integer\" },\n        \"created_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"note\": { \"type\": [\"string\", \"null\"] },\n        \"restock\": { \"type\": \"boolean\" },\n        \"refund_line_items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\"\
  : {\n              \"id\": { \"type\": \"integer\" },\n              \"quantity\": { \"type\": \"integer\" },\n              \"line_item_id\": { \"type\": \"integer\" },\n              \"subtotal\": { \"type\": \"number\" },\n              \"total_tax\": { \"type\": \"number\" }\n            }\n          }\n        },\n        \"admin_graphql_api_id\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/json-schema/shopify-order-schema.json
tags:
- Commerce
- Ecommerce
- Payments
- Retail
- Shopping Cart
- T1
title: Shopify Order
---
