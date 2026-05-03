---
description: Schema for an Oracle Retail OMS customer order across omnichannel fulfillment.
layout: schema
name: Oracle Retail Order
properties_list:
- description: System-generated order identifier
  name: orderId
  type: string
- description: Order ID from originating channel system
  name: externalOrderId
  type: string
- description: Current order status
  name: status
  type: string
- description: Sales channel identifier (e.g., WEB, STORE, MOBILE)
  name: channelId
  type: string
- description: Customer identifier
  name: customerId
  type: string
- description: Date and time the order was placed
  name: orderDate
  type: string
- description: ISO 4217 currency code
  name: currencyCode
  type: string
- description: Order subtotal before tax and shipping
  name: subtotal
  type: number
- description: Total tax amount
  name: taxTotal
  type: number
- description: Total shipping and handling
  name: shippingTotal
  type: number
- description: Total discount amount
  name: discountTotal
  type: number
- description: Grand total (subtotal + tax + shipping - discounts)
  name: orderTotal
  type: number
- description: ''
  name: shippingAddress
  type: object
- description: ''
  name: billingAddress
  type: object
- description: ''
  name: lines
  type: array
- description: ''
  name: createDatetime
  type: string
- description: ''
  name: lastUpdateDatetime
  type: string
provider_name: Oracle Retail
provider_slug: oracle-retail
schema_file: json-schema/oracle-retail-order-schema.json
slug: oracle-retail-order
source_filename: oracle-retail-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/oracle-retail/json-schema/oracle-retail-order-schema.json\",\n  \"title\": \"Oracle Retail Order\",\n  \"description\": \"Schema for an Oracle Retail OMS customer order across omnichannel fulfillment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated order identifier\"\n    },\n    \"externalOrderId\": {\n      \"type\": \"string\",\n      \"description\": \"Order ID from originating channel system\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"CREATED\", \"PAYMENT_PENDING\", \"CONFIRMED\", \"PROCESSING\", \"SHIPPED\", \"DELIVERED\", \"CANCELLED\", \"RETURNED\"],\n      \"description\": \"Current order status\"\n    },\n    \"channelId\": {\n      \"type\": \"string\",\n      \"description\": \"Sales channel identifier (e.g., WEB, STORE, MOBILE)\"\
  \n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Customer identifier\"\n    },\n    \"orderDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the order was placed\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"minLength\": 3,\n      \"maxLength\": 3,\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"subtotal\": {\n      \"type\": \"number\",\n      \"description\": \"Order subtotal before tax and shipping\"\n    },\n    \"taxTotal\": {\n      \"type\": \"number\",\n      \"description\": \"Total tax amount\"\n    },\n    \"shippingTotal\": {\n      \"type\": \"number\",\n      \"description\": \"Total shipping and handling\"\n    },\n    \"discountTotal\": {\n      \"type\": \"number\",\n      \"description\": \"Total discount amount\"\n    },\n    \"orderTotal\": {\n      \"type\": \"number\",\n      \"description\": \"Grand total (subtotal + tax\
  \ + shipping - discounts)\"\n    },\n    \"shippingAddress\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"billingAddress\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"lines\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/OrderLine\"\n      }\n    },\n    \"createDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastUpdateDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"orderId\", \"status\", \"channelId\", \"customerId\", \"orderDate\"],\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"firstName\": { \"type\": \"string\" },\n        \"lastName\": { \"type\": \"string\" },\n        \"address1\": { \"type\": \"string\" },\n        \"address2\": { \"type\": \"string\" },\n        \"city\": { \"type\": \"string\" },\n        \"state\": { \"type\": \"string\" },\n        \"postalCode\"\
  : { \"type\": \"string\" },\n        \"country\": { \"type\": \"string\", \"maxLength\": 3 },\n        \"phone\": { \"type\": \"string\" },\n        \"email\": { \"type\": \"string\", \"format\": \"email\" }\n      },\n      \"required\": [\"address1\", \"city\", \"country\"]\n    },\n    \"OrderLine\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"lineId\": { \"type\": \"string\" },\n        \"itemId\": { \"type\": \"string\" },\n        \"itemDescription\": { \"type\": \"string\" },\n        \"quantity\": { \"type\": \"integer\", \"minimum\": 1 },\n        \"unitPrice\": { \"type\": \"number\" },\n        \"lineTotal\": { \"type\": \"number\" },\n        \"status\": { \"type\": \"string\" },\n        \"fulfillmentType\": {\n          \"type\": \"string\",\n          \"enum\": [\"SHIP_TO_HOME\", \"SHIP_TO_STORE\", \"PICKUP_IN_STORE\", \"DELIVERY\"]\n        }\n      },\n      \"required\": [\"lineId\", \"itemId\", \"quantity\", \"unitPrice\"]\n    }\n  },\n  \"examples\"\
  : [\n    {\n      \"orderId\": \"ORD-2026-00123456\",\n      \"externalOrderId\": \"WEB-20260315-9872\",\n      \"status\": \"CONFIRMED\",\n      \"channelId\": \"WEB\",\n      \"customerId\": \"CUST-10045\",\n      \"orderDate\": \"2026-03-15T14:23:00Z\",\n      \"currencyCode\": \"USD\",\n      \"subtotal\": 74.97,\n      \"taxTotal\": 6.00,\n      \"shippingTotal\": 5.99,\n      \"discountTotal\": 0.00,\n      \"orderTotal\": 86.96\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/json-schema/oracle-retail-order-schema.json
tags:
- Retail
- Merchandising
- Order Management
- Pricing
- Inventory
- Point of Sale
- Omnichannel
- Oracle
title: Oracle Retail Order
---
