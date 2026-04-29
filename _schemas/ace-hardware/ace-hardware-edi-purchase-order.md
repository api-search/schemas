---
description: An Ace Hardware EDI 850 Purchase Order representing a vendor purchase order from Ace Hardware's distribution system.
layout: schema
name: AceHardwareEdiPurchaseOrder
properties_list:
- description: Purchase order number assigned by Ace Hardware
  name: poNumber
  type: string
- description: Date the purchase order was created
  name: orderDate
  type: string
- description: Required ship-by date for the order
  name: shipByDate
  type: string
- description: Ace Hardware vendor identifier
  name: vendorId
  type: string
- description: Name of the vendor fulfilling the order
  name: vendorName
  type: string
- description: Destination distribution center or store address
  name: shipToAddress
  type: object
- description: List of products ordered
  name: lineItems
  type: array
- description: Total order value in USD
  name: totalAmount
  type: number
- description: Currency code
  name: currency
  type: string
provider_name: Ace Hardware
provider_slug: ace-hardware
schema_file: json-schema/ace-hardware-edi-purchase-order-schema.json
slug: ace-hardware-edi-purchase-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ace-hardware/refs/heads/main/json-schema/ace-hardware-edi-purchase-order-schema.json\",\n  \"title\": \"AceHardwareEdiPurchaseOrder\",\n  \"description\": \"An Ace Hardware EDI 850 Purchase Order representing a vendor purchase order from Ace Hardware's distribution system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"poNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Purchase order number assigned by Ace Hardware\",\n      \"example\": \"PO-2026-001234\"\n    },\n    \"orderDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the purchase order was created\",\n      \"example\": \"2026-04-19\"\n    },\n    \"shipByDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Required ship-by date for the order\",\n      \"example\": \"2026-04-30\"\
  \n    },\n    \"vendorId\": {\n      \"type\": \"string\",\n      \"description\": \"Ace Hardware vendor identifier\",\n      \"example\": \"VND-00987\"\n    },\n    \"vendorName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the vendor fulfilling the order\",\n      \"example\": \"Hardware Supplier Corp.\"\n    },\n    \"shipToAddress\": {\n      \"type\": \"object\",\n      \"description\": \"Destination distribution center or store address\",\n      \"properties\": {\n        \"name\": {\"type\": \"string\", \"example\": \"Ace Hardware DC - Chicago\"},\n        \"address1\": {\"type\": \"string\", \"example\": \"1000 Distribution Way\"},\n        \"city\": {\"type\": \"string\", \"example\": \"Chicago\"},\n        \"state\": {\"type\": \"string\", \"example\": \"IL\"},\n        \"zip\": {\"type\": \"string\", \"example\": \"60601\"},\n        \"country\": {\"type\": \"string\", \"example\": \"US\"}\n      }\n    },\n    \"lineItems\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"List of products ordered\",\n      \"items\": {\n        \"$ref\": \"#/$defs/LineItem\"\n      }\n    },\n    \"totalAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Total order value in USD\",\n      \"example\": 15420.50\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code\",\n      \"example\": \"USD\"\n    }\n  },\n  \"required\": [\"poNumber\", \"orderDate\", \"vendorId\", \"lineItems\"],\n  \"$defs\": {\n    \"LineItem\": {\n      \"type\": \"object\",\n      \"description\": \"A single line item in a purchase order\",\n      \"properties\": {\n        \"lineNumber\": {\"type\": \"integer\", \"description\": \"Sequential line item number\", \"example\": 1},\n        \"upc\": {\"type\": \"string\", \"description\": \"Universal Product Code\", \"example\": \"012345678901\"},\n        \"vendorSku\": {\"type\": \"string\", \"description\": \"Vendor's product SKU\", \"example\": \"SKU-HAMMER-16OZ\"\
  },\n        \"aceItemNumber\": {\"type\": \"string\", \"description\": \"Ace Hardware internal item number\", \"example\": \"4082165\"},\n        \"description\": {\"type\": \"string\", \"description\": \"Product description\", \"example\": \"16 oz Claw Hammer\"},\n        \"quantity\": {\"type\": \"integer\", \"description\": \"Quantity ordered\", \"example\": 48},\n        \"unitCost\": {\"type\": \"number\", \"description\": \"Cost per unit in USD\", \"example\": 12.99},\n        \"extendedCost\": {\"type\": \"number\", \"description\": \"Total line cost (quantity x unitCost)\", \"example\": 623.52}\n      },\n      \"required\": [\"lineNumber\", \"upc\", \"quantity\", \"unitCost\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ace-hardware/refs/heads/main/json-schema/ace-hardware-edi-purchase-order-schema.json
tags:
- Retail
- Hardware
- Home Improvement
- Tools
- Paint
- Cooperative
- EDI
- Affiliate
title: AceHardwareEdiPurchaseOrder
---
