---
description: An omnichannel order managed by Manhattan Active Omni
layout: schema
name: Manhattan Active Order
properties_list:
- description: Internal order identifier
  name: orderId
  type: string
- description: Channel or customer order number
  name: externalOrderId
  type: string
- description: ''
  name: status
  type: string
- description: Originating sales channel identifier
  name: channelId
  type: string
- description: ''
  name: customerId
  type: string
- description: ''
  name: orderDate
  type: string
- description: ''
  name: requiredDeliveryDate
  type: string
- description: ''
  name: shippingAddress
  type: object
- description: ''
  name: lines
  type: array
- description: ''
  name: totals
  type: object
- description: ''
  name: fulfillments
  type: array
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: manhattan-associates
provider_slug: manhattan-associates
schema_file: json-schema/manhattan-associates-order-schema.json
slug: manhattan-associates-order
source_filename: manhattan-associates-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/manhattan-associates/refs/heads/main/json-schema/manhattan-associates-order-schema.json\",\n  \"title\": \"Manhattan Active Order\",\n  \"description\": \"An omnichannel order managed by Manhattan Active Omni\",\n  \"type\": \"object\",\n  \"required\": [\"orderId\", \"channelId\", \"customerId\", \"status\", \"lines\"],\n  \"properties\": {\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"Internal order identifier\"\n    },\n    \"externalOrderId\": {\n      \"type\": \"string\",\n      \"description\": \"Channel or customer order number\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"created\", \"allocated\", \"released\", \"shipped\", \"delivered\", \"cancelled\", \"returned\"]\n    },\n    \"channelId\": {\n      \"type\": \"string\",\n      \"description\": \"Originating sales channel\
  \ identifier\"\n    },\n    \"customerId\": {\n      \"type\": \"string\"\n    },\n    \"orderDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"requiredDeliveryDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"shippingAddress\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"lines\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/OrderLine\"\n      }\n    },\n    \"totals\": {\n      \"$ref\": \"#/$defs/OrderTotals\"\n    },\n    \"fulfillments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Fulfillment\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$defs\": {\n    \"OrderLine\": {\n      \"type\": \"object\",\n      \"required\": [\"lineId\", \"itemId\", \"quantity\"\
  ],\n      \"properties\": {\n        \"lineId\": { \"type\": \"string\" },\n        \"externalLineId\": { \"type\": \"string\" },\n        \"itemId\": { \"type\": \"string\" },\n        \"sku\": { \"type\": \"string\" },\n        \"description\": { \"type\": \"string\" },\n        \"quantity\": { \"type\": \"number\", \"minimum\": 0 },\n        \"unitPrice\": { \"type\": \"number\", \"minimum\": 0 },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"open\", \"allocated\", \"released\", \"shipped\", \"delivered\", \"cancelled\"]\n        },\n        \"fulfillmentNodeId\": { \"type\": \"string\" }\n      }\n    },\n    \"OrderTotals\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"subtotal\": { \"type\": \"number\" },\n        \"taxTotal\": { \"type\": \"number\" },\n        \"shippingTotal\": { \"type\": \"number\" },\n        \"discountTotal\": { \"type\": \"number\" },\n        \"orderTotal\": { \"type\": \"number\" },\n        \"currency\"\
  : { \"type\": \"string\", \"default\": \"USD\" }\n      }\n    },\n    \"Fulfillment\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"fulfillmentId\": { \"type\": \"string\" },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"ship_from_store\", \"ship_from_dc\", \"in_store_pickup\", \"curbside_pickup\"]\n        },\n        \"nodeId\": { \"type\": \"string\" },\n        \"nodeName\": { \"type\": \"string\" },\n        \"status\": { \"type\": \"string\" },\n        \"trackingNumber\": { \"type\": \"string\" },\n        \"carrier\": { \"type\": \"string\" },\n        \"estimatedDeliveryDate\": { \"type\": \"string\", \"format\": \"date\" },\n        \"shippedAt\": { \"type\": \"string\", \"format\": \"date-time\" }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"required\": [\"street1\", \"city\", \"state\", \"postalCode\", \"country\"],\n      \"properties\": {\n        \"firstName\": { \"type\": \"string\" },\n\
  \        \"lastName\": { \"type\": \"string\" },\n        \"street1\": { \"type\": \"string\" },\n        \"street2\": { \"type\": \"string\" },\n        \"city\": { \"type\": \"string\" },\n        \"state\": { \"type\": \"string\" },\n        \"postalCode\": { \"type\": \"string\" },\n        \"country\": { \"type\": \"string\" },\n        \"phone\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/manhattan-associates/refs/heads/main/json-schema/manhattan-associates-order-schema.json
tags: []
title: Manhattan Active Order
---
