---
description: A sales order in the ScanSource technology distribution platform, representing a purchase transaction between a partner and ScanSource.
layout: schema
name: ScanSource Sales Order
properties_list:
- description: ScanSource assigned sales order number
  name: salesOrderNumber
  type: string
- description: Customer purchase order number
  name: poNumber
  type: string
- description: ScanSource customer account number
  name: customerNumber
  type: string
- description: Current order status
  name: status
  type: string
- description: Date and time the order was placed
  name: orderDate
  type: string
- description: Identifier of the person who placed the order
  name: requestor
  type: string
- description: Shipping destination address
  name: shipToAddress
  type: object
- description: Carrier and service level code
  name: shippingMethod
  type: string
- description: List of products ordered
  name: lineItems
  type: array
- description: Total order amount
  name: totalAmount
  type: number
- description: Currency code
  name: currency
  type: string
- description: Carrier tracking information
  name: tracking
  type: array
provider_name: ScanSource
provider_slug: scansource
schema_file: json-schema/scansource-order-schema.json
slug: scansource-order
source_filename: scansource-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://github.com/api-evangelist/scansource/blob/main/json-schema/scansource-order-schema.json\",\n  \"title\": \"ScanSource Sales Order\",\n  \"description\": \"A sales order in the ScanSource technology distribution platform, representing a purchase transaction between a partner and ScanSource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"salesOrderNumber\": {\n      \"type\": \"string\",\n      \"description\": \"ScanSource assigned sales order number\"\n    },\n    \"poNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Customer purchase order number\"\n    },\n    \"customerNumber\": {\n      \"type\": \"string\",\n      \"description\": \"ScanSource customer account number\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current order status\",\n      \"enum\": [\"Pending\", \"Processing\", \"Shipped\", \"Delivered\", \"Cancelled\"\
  , \"OnHold\"]\n    },\n    \"orderDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the order was placed\"\n    },\n    \"requestor\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the person who placed the order\"\n    },\n    \"shipToAddress\": {\n      \"type\": \"object\",\n      \"description\": \"Shipping destination address\",\n      \"properties\": {\n        \"name\": { \"type\": \"string\" },\n        \"address1\": { \"type\": \"string\" },\n        \"address2\": { \"type\": \"string\" },\n        \"city\": { \"type\": \"string\" },\n        \"state\": { \"type\": \"string\" },\n        \"postalCode\": { \"type\": \"string\" },\n        \"country\": { \"type\": \"string\", \"default\": \"US\" }\n      },\n      \"required\": [\"address1\", \"city\", \"state\", \"postalCode\"]\n    },\n    \"shippingMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Carrier and service level\
  \ code\"\n    },\n    \"lineItems\": {\n      \"type\": \"array\",\n      \"description\": \"List of products ordered\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"lineNumber\": { \"type\": \"integer\" },\n          \"itemNumber\": { \"type\": \"string\" },\n          \"manufacturerPartNumber\": { \"type\": \"string\" },\n          \"description\": { \"type\": \"string\" },\n          \"quantity\": { \"type\": \"integer\", \"minimum\": 1 },\n          \"unitPrice\": { \"type\": \"number\" },\n          \"extendedPrice\": { \"type\": \"number\" },\n          \"status\": { \"type\": \"string\" }\n        },\n        \"required\": [\"itemNumber\", \"quantity\"]\n      }\n    },\n    \"totalAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Total order amount\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"default\": \"USD\",\n      \"description\": \"Currency code\"\n    },\n    \"tracking\": {\n      \"\
  type\": \"array\",\n      \"description\": \"Carrier tracking information\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"trackingNumber\": { \"type\": \"string\" },\n          \"carrier\": { \"type\": \"string\" },\n          \"status\": { \"type\": \"string\" },\n          \"estimatedDelivery\": { \"type\": \"string\", \"format\": \"date\" }\n        }\n      }\n    }\n  },\n  \"required\": [\"poNumber\", \"lineItems\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/json-schema/scansource-order-schema.json
tags:
- ScanSource
- Distribution
- Barcode
- Point Of Sale
- AIDC
- Inventory
- Order Management
- E-Commerce
title: ScanSource Sales Order
---
