---
description: Schema for a Rithum Dsco platform order, used in dropship and marketplace commerce integrations.
layout: schema
name: Dsco Order
properties_list:
- description: Unique order identifier assigned by the Dsco platform
  name: orderId
  type: string
- description: Indicates whether this is a dropship or marketplace order
  name: orderType
  type: string
- description: Current status of the order
  name: status
  type: string
- description: Timestamp when the order was created
  name: createdAt
  type: string
- description: Timestamp when the order was last updated
  name: updatedAt
  type: string
- description: Identifier of the retailer who placed the order
  name: retailerId
  type: string
- description: Identifier of the supplier fulfilling the order
  name: supplierId
  type: string
- description: Line items included in the order
  name: items
  type: array
- description: Shipping destination address
  name: shippingAddress
  type: object
provider_name: Rithum
provider_slug: rithum
schema_file: json-schema/dsco-order-schema.json
slug: dsco-order
source_filename: dsco-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/rithum/json-schema/dsco-order-schema.json\",\n  \"title\": \"Dsco Order\",\n  \"description\": \"Schema for a Rithum Dsco platform order, used in dropship and marketplace commerce integrations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique order identifier assigned by the Dsco platform\"\n    },\n    \"orderType\": {\n      \"type\": \"string\",\n      \"enum\": [\"Dropship\", \"Marketplace\"],\n      \"description\": \"Indicates whether this is a dropship or marketplace order\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the order\",\n      \"enum\": [\"pending\", \"acknowledged\", \"shipped\", \"cancelled\", \"returned\", \"invoiced\"]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"Timestamp when the order was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the order was last updated\"\n    },\n    \"retailerId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the retailer who placed the order\"\n    },\n    \"supplierId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the supplier fulfilling the order\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Line items included in the order\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"lineItemId\", \"sku\", \"quantity\"],\n        \"properties\": {\n          \"lineItemId\": {\n            \"type\": \"string\",\n            \"description\": \"Unique line item identifier\"\n          },\n          \"sku\": {\n            \"type\": \"string\",\n            \"description\": \"Supplier stock\
  \ keeping unit\"\n          },\n          \"quantity\": {\n            \"type\": \"integer\",\n            \"minimum\": 1,\n            \"description\": \"Ordered quantity\"\n          },\n          \"cost\": {\n            \"type\": \"number\",\n            \"format\": \"float\",\n            \"description\": \"Wholesale cost charged by supplier to retailer\"\n          },\n          \"price\": {\n            \"type\": \"number\",\n            \"format\": \"float\",\n            \"description\": \"Retail price\"\n          }\n        }\n      }\n    },\n    \"shippingAddress\": {\n      \"type\": \"object\",\n      \"description\": \"Shipping destination address\",\n      \"properties\": {\n        \"name\": { \"type\": \"string\" },\n        \"street1\": { \"type\": \"string\" },\n        \"street2\": { \"type\": \"string\" },\n        \"city\": { \"type\": \"string\" },\n        \"state\": { \"type\": \"string\" },\n        \"postalCode\": { \"type\": \"string\" },\n        \"country\"\
  : { \"type\": \"string\" },\n        \"phone\": { \"type\": \"string\" }\n      },\n      \"required\": [\"name\", \"street1\", \"city\", \"state\", \"postalCode\", \"country\"]\n    }\n  },\n  \"required\": [\"orderId\", \"orderType\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rithum/refs/heads/main/json-schema/dsco-order-schema.json
tags:
- Commerce
- Dropship
- Marketplace
- Ecommerce
- Supply Chain
- Retail
title: Dsco Order
---
