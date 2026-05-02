---
description: A sales order in Adobe Commerce (Magento). Represents a completed purchase transaction including the customer, line items, billing and shipping addresses, payment method, and all financial totals. Orders are created from shopping cart quotes and progress through a lifecycle of states including new, processing, complete, closed, and canceled.
layout: schema
name: Magento Order
properties_list:
- description: Numeric order entity ID assigned by Commerce. Read-only after creation.
  name: entity_id
  type: integer
- description: Human-readable order number displayed to merchants and customers (e.g. 000000001). Zero-padded numeric string determined by the store's order ID prefix and increment settings.
  name: increment_id
  type: string
- description: Numeric store view entity ID indicating which store view the order was placed through.
  name: store_id
  type: integer
- description: Current order status code. Merchants can define custom statuses in addition to the built-in defaults.
  name: status
  type: string
- description: Internal state machine state of the order. States are a smaller set than statuses and drive available actions on the order.
  name: state
  type: string
- description: Numeric customer entity ID. Null for guest orders.
  name: customer_id
  type:
  - integer
  - 'null'
- description: Email address of the customer or guest who placed the order. Required for both registered and guest orders.
  name: customer_email
  type: string
- description: Customer first name as entered during checkout.
  name: customer_firstname
  type: string
- description: Customer last name as entered during checkout.
  name: customer_lastname
  type: string
- description: Whether the order was placed by a guest shopper (not a registered customer account).
  name: customer_is_guest
  type: boolean
- description: Customer group ID at the time of order placement. Affects pricing, tax, and shipping rules applied.
  name: customer_group_id
  type: integer
- description: ISO 8601 timestamp in UTC when the order was created.
  name: created_at
  type: string
- description: ISO 8601 timestamp in UTC when the order record was last modified.
  name: updated_at
  type: string
- description: Order grand total including subtotal, tax, shipping, and applied discounts. In the order's display currency.
  name: grand_total
  type: number
- description: Sum of line item row totals before tax, shipping, and discounts.
  name: subtotal
  type: number
- description: Total tax amount applied to the order.
  name: tax_amount
  type: number
- description: Shipping fee charged on the order before any shipping discounts.
  name: shipping_amount
  type: number
- description: Total discount amount applied to the order from cart price rules and coupon codes. Typically a negative value.
  name: discount_amount
  type: number
- description: ISO 4217 currency code for the store's base currency used in base_grand_total and base_* fields.
  name: base_currency_code
  type: string
- description: ISO 4217 currency code in which the order was placed and displayed to the customer.
  name: order_currency_code
  type: string
- description: Coupon code applied to the order, if any.
  name: coupon_code
  type: string
- description: Carrier and method code for the selected shipping method (e.g. flatrate_flatrate, ups_ground).
  name: shipping_method
  type: string
- description: Human-readable shipping method description shown to the customer.
  name: shipping_description
  type: string
- description: Billing address used for payment authorization.
  name: billing_address
  type: object
- description: Extension attributes provided by Commerce modules. Common extension attributes include shipping_assignments for multi-address orders and payment_additional_info for payment gateway data.
  name: extension_attributes
  type: object
- description: Line items in the order. Each item represents a purchased product with its quantity, pricing, and fulfillment status.
  name: items
  type: array
- description: Chronological history of order status changes and admin comments.
  name: status_histories
  type: array
- description: Payment method and transaction details for the order.
  name: payment
  type: object
provider_name: magento
provider_slug: magento
schema_file: json-schema/magento-order-schema.json
slug: magento-order
source_filename: magento-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/magento/schemas/magento-order.json\",\n  \"title\": \"Magento Order\",\n  \"description\": \"A sales order in Adobe Commerce (Magento). Represents a completed purchase transaction including the customer, line items, billing and shipping addresses, payment method, and all financial totals. Orders are created from shopping cart quotes and progress through a lifecycle of states including new, processing, complete, closed, and canceled.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"increment_id\",\n    \"status\",\n    \"state\",\n    \"customer_email\",\n    \"grand_total\",\n    \"items\",\n    \"billing_address\"\n  ],\n  \"properties\": {\n    \"entity_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric order entity ID assigned by Commerce. Read-only after creation.\"\n    },\n    \"increment_id\": {\n      \"type\": \"string\",\n  \
  \    \"description\": \"Human-readable order number displayed to merchants and customers (e.g. 000000001). Zero-padded numeric string determined by the store's order ID prefix and increment settings.\",\n      \"pattern\": \"^[0-9]+$\"\n    },\n    \"store_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric store view entity ID indicating which store view the order was placed through.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current order status code. Merchants can define custom statuses in addition to the built-in defaults.\",\n      \"enum\": [\n        \"pending\",\n        \"pending_payment\",\n        \"processing\",\n        \"complete\",\n        \"closed\",\n        \"canceled\",\n        \"holded\",\n        \"payment_review\",\n        \"fraud\"\n      ]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Internal state machine state of the order. States are a smaller set than statuses\
  \ and drive available actions on the order.\",\n      \"enum\": [\n        \"new\",\n        \"pending_payment\",\n        \"processing\",\n        \"complete\",\n        \"closed\",\n        \"canceled\",\n        \"holded\",\n        \"payment_review\"\n      ]\n    },\n    \"customer_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Numeric customer entity ID. Null for guest orders.\"\n    },\n    \"customer_email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the customer or guest who placed the order. Required for both registered and guest orders.\",\n      \"maxLength\": 255\n    },\n    \"customer_firstname\": {\n      \"type\": \"string\",\n      \"description\": \"Customer first name as entered during checkout.\",\n      \"maxLength\": 255\n    },\n    \"customer_lastname\": {\n      \"type\": \"string\",\n      \"description\": \"Customer last name as entered during checkout.\",\n      \"maxLength\"\
  : 255\n    },\n    \"customer_is_guest\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the order was placed by a guest shopper (not a registered customer account).\"\n    },\n    \"customer_group_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Customer group ID at the time of order placement. Affects pricing, tax, and shipping rules applied.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp in UTC when the order was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp in UTC when the order record was last modified.\"\n    },\n    \"grand_total\": {\n      \"type\": \"number\",\n      \"description\": \"Order grand total including subtotal, tax, shipping, and applied discounts. In the order's display currency.\",\n      \"minimum\": 0\n    },\n    \"subtotal\": {\n\
  \      \"type\": \"number\",\n      \"description\": \"Sum of line item row totals before tax, shipping, and discounts.\",\n      \"minimum\": 0\n    },\n    \"tax_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Total tax amount applied to the order.\",\n      \"minimum\": 0\n    },\n    \"shipping_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Shipping fee charged on the order before any shipping discounts.\",\n      \"minimum\": 0\n    },\n    \"discount_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Total discount amount applied to the order from cart price rules and coupon codes. Typically a negative value.\",\n      \"maximum\": 0\n    },\n    \"base_currency_code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for the store's base currency used in base_grand_total and base_* fields.\",\n      \"minLength\": 3,\n      \"maxLength\": 3\n    },\n    \"order_currency_code\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"ISO 4217 currency code in which the order was placed and displayed to the customer.\",\n      \"minLength\": 3,\n      \"maxLength\": 3\n    },\n    \"coupon_code\": {\n      \"type\": \"string\",\n      \"description\": \"Coupon code applied to the order, if any.\",\n      \"maxLength\": 255\n    },\n    \"shipping_method\": {\n      \"type\": \"string\",\n      \"description\": \"Carrier and method code for the selected shipping method (e.g. flatrate_flatrate, ups_ground).\",\n      \"maxLength\": 120\n    },\n    \"shipping_description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable shipping method description shown to the customer.\",\n      \"maxLength\": 255\n    },\n    \"billing_address\": {\n      \"$ref\": \"#/$defs/Address\",\n      \"description\": \"Billing address used for payment authorization.\"\n    },\n    \"extension_attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Extension attributes\
  \ provided by Commerce modules. Common extension attributes include shipping_assignments for multi-address orders and payment_additional_info for payment gateway data.\",\n      \"additionalProperties\": true\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Line items in the order. Each item represents a purchased product with its quantity, pricing, and fulfillment status.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/OrderItem\"\n      }\n    },\n    \"status_histories\": {\n      \"type\": \"array\",\n      \"description\": \"Chronological history of order status changes and admin comments.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/StatusHistory\"\n      }\n    },\n    \"payment\": {\n      \"$ref\": \"#/$defs/Payment\",\n      \"description\": \"Payment method and transaction details for the order.\"\n    }\n  },\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A postal address\
  \ for billing or shipping. Used within orders, customers, and quote objects.\",\n      \"required\": [\n        \"firstname\",\n        \"lastname\",\n        \"street\",\n        \"city\",\n        \"country_id\",\n        \"postcode\",\n        \"telephone\"\n      ],\n      \"properties\": {\n        \"address_type\": {\n          \"type\": \"string\",\n          \"description\": \"Whether this is a billing or shipping address.\",\n          \"enum\": [\"billing\", \"shipping\"]\n        },\n        \"firstname\": {\n          \"type\": \"string\",\n          \"description\": \"First name of the address recipient.\",\n          \"maxLength\": 255\n        },\n        \"lastname\": {\n          \"type\": \"string\",\n          \"description\": \"Last name of the address recipient.\",\n          \"maxLength\": 255\n        },\n        \"company\": {\n          \"type\": \"string\",\n          \"description\": \"Company name, if applicable.\",\n          \"maxLength\": 255\n        },\n\
  \        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address associated with this address.\"\n        },\n        \"street\": {\n          \"type\": \"array\",\n          \"description\": \"Street address lines. The first element is the primary street line; additional elements are continuation lines.\",\n          \"minItems\": 1,\n          \"maxItems\": 4,\n          \"items\": {\n            \"type\": \"string\",\n            \"maxLength\": 255\n          }\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City or municipality name.\",\n          \"maxLength\": 255\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"State, province, or region name.\",\n          \"maxLength\": 255\n        },\n        \"region_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Numeric Commerce region ID for the state\
  \ or province.\"\n        },\n        \"region_code\": {\n          \"type\": \"string\",\n          \"description\": \"Abbreviated state or province code (e.g. CA, NY, TX).\",\n          \"maxLength\": 32\n        },\n        \"country_id\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 3166-1 alpha-2 two-letter country code.\",\n          \"minLength\": 2,\n          \"maxLength\": 2,\n          \"pattern\": \"^[A-Z]{2}$\"\n        },\n        \"postcode\": {\n          \"type\": \"string\",\n          \"description\": \"Postal code or ZIP code.\",\n          \"maxLength\": 255\n        },\n        \"telephone\": {\n          \"type\": \"string\",\n          \"description\": \"Phone number for the address.\",\n          \"maxLength\": 255\n        }\n      }\n    },\n    \"OrderItem\": {\n      \"type\": \"object\",\n      \"description\": \"A product line item within a sales order.\",\n      \"required\": [\n        \"sku\",\n        \"name\",\n        \"qty_ordered\"\
  ,\n        \"price\",\n        \"product_type\"\n      ],\n      \"properties\": {\n        \"item_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Numeric order item entity ID.\"\n        },\n        \"order_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Numeric entity ID of the parent order.\"\n        },\n        \"sku\": {\n          \"type\": \"string\",\n          \"description\": \"Product SKU at the time of purchase.\",\n          \"maxLength\": 64\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Product name at the time of purchase.\",\n          \"maxLength\": 255\n        },\n        \"product_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Numeric product entity ID.\"\n        },\n        \"product_type\": {\n          \"type\": \"string\",\n          \"description\": \"Product type at the time of purchase.\",\n          \"enum\": [\"simple\", \"configurable\"\
  , \"virtual\", \"downloadable\", \"bundle\", \"grouped\"]\n        },\n        \"qty_ordered\": {\n          \"type\": \"number\",\n          \"description\": \"Total quantity ordered for this item.\",\n          \"minimum\": 0\n        },\n        \"qty_invoiced\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity that has been invoiced.\",\n          \"minimum\": 0\n        },\n        \"qty_shipped\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity that has been shipped.\",\n          \"minimum\": 0\n        },\n        \"qty_refunded\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity that has been refunded via credit memo.\",\n          \"minimum\": 0\n        },\n        \"qty_canceled\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity that has been canceled.\",\n          \"minimum\": 0\n        },\n        \"price\": {\n          \"type\": \"number\",\n          \"description\"\
  : \"Unit price of the product inclusive of any tier pricing applied.\",\n          \"minimum\": 0\n        },\n        \"original_price\": {\n          \"type\": \"number\",\n          \"description\": \"Original catalog price before any discounts or rules were applied.\",\n          \"minimum\": 0\n        },\n        \"row_total\": {\n          \"type\": \"number\",\n          \"description\": \"Line total: unit price multiplied by quantity ordered.\",\n          \"minimum\": 0\n        },\n        \"tax_amount\": {\n          \"type\": \"number\",\n          \"description\": \"Tax amount applied to this line item.\",\n          \"minimum\": 0\n        },\n        \"tax_percent\": {\n          \"type\": \"number\",\n          \"description\": \"Tax percentage rate applied to this item.\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        },\n        \"discount_amount\": {\n          \"type\": \"number\",\n          \"description\": \"Discount amount applied to this line\
  \ item.\",\n          \"minimum\": 0\n        },\n        \"weight\": {\n          \"type\": \"number\",\n          \"description\": \"Product weight used for shipping calculation.\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"Payment\": {\n      \"type\": \"object\",\n      \"description\": \"Payment method details and transaction information for an order.\",\n      \"required\": [\n        \"method\"\n      ],\n      \"properties\": {\n        \"entity_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Numeric payment entity ID.\"\n        },\n        \"parent_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Numeric order entity ID this payment belongs to.\"\n        },\n        \"method\": {\n          \"type\": \"string\",\n          \"description\": \"Payment method code (e.g. checkmo, braintree, free, payflowpro).\",\n          \"maxLength\": 128\n        },\n        \"amount_ordered\": {\n          \"type\": \"number\"\
  ,\n          \"description\": \"Payment amount to collect equal to the order grand total.\",\n          \"minimum\": 0\n        },\n        \"amount_paid\": {\n          \"type\": \"number\",\n          \"description\": \"Amount that has been captured from the payment method.\",\n          \"minimum\": 0\n        },\n        \"amount_authorized\": {\n          \"type\": \"number\",\n          \"description\": \"Amount authorized but not yet captured.\",\n          \"minimum\": 0\n        },\n        \"last_trans_id\": {\n          \"type\": \"string\",\n          \"description\": \"Transaction ID from the payment gateway for the most recent transaction.\"\n        },\n        \"cc_last4\": {\n          \"type\": \"string\",\n          \"description\": \"Last four digits of the credit card number, if applicable.\",\n          \"pattern\": \"^[0-9]{4}$\"\n        }\n      }\n    },\n    \"StatusHistory\": {\n      \"type\": \"object\",\n      \"description\": \"An entry in the order status\
  \ history log.\",\n      \"properties\": {\n        \"entity_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Numeric status history entity ID.\"\n        },\n        \"parent_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Numeric order entity ID this history entry belongs to.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Order status code at the time this history entry was created.\"\n        },\n        \"comment\": {\n          \"type\": \"string\",\n          \"description\": \"Admin or system comment text for this history entry.\"\n        },\n        \"is_customer_notified\": {\n          \"type\": \"integer\",\n          \"description\": \"Whether the customer was notified by email for this history entry. 1 = yes, 0 = no.\",\n          \"enum\": [0, 1]\n        },\n        \"is_visible_on_front\": {\n          \"type\": \"integer\",\n          \"description\": \"Whether this comment\
  \ is visible to the customer in their account. 1 = yes, 0 = no.\",\n          \"enum\": [0, 1]\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when this history entry was created.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/json-schema/magento-order-schema.json
tags: []
title: Magento Order
---
