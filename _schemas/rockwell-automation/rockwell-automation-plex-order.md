---
description: Schema representing a customer order in the Plex Smart Manufacturing Platform ERP API.
layout: schema
name: Rockwell Automation Plex Customer Order
properties_list:
- description: Unique order identifier in Plex ERP
  name: orderId
  type: string
- description: Human-readable order number
  name: orderNumber
  type: string
- description: Customer identifier in Plex
  name: customerId
  type: string
- description: Customer name
  name: customerName
  type: string
- description: Date the order was placed
  name: orderDate
  type: string
- description: Requested delivery date
  name: dueDate
  type: string
- description: Current order status
  name: status
  type: string
- description: Order fulfillment priority
  name: priority
  type: string
- description: Line items in the order
  name: orderLines
  type: array
- description: Delivery address
  name: shippingAddress
  type: object
- description: Order notes or special instructions
  name: notes
  type: string
provider_name: Rockwell Automation
provider_slug: rockwell-automation
schema_file: json-schema/rockwell-automation-plex-order-schema.json
slug: rockwell-automation-plex-order
source_filename: rockwell-automation-plex-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/rockwell-automation/json-schema/rockwell-automation-plex-order-schema.json\",\n  \"title\": \"Rockwell Automation Plex Customer Order\",\n  \"description\": \"Schema representing a customer order in the Plex Smart Manufacturing Platform ERP API.\",\n  \"type\": \"object\",\n  \"required\": [\"customerId\", \"orderDate\", \"orderLines\"],\n  \"properties\": {\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique order identifier in Plex ERP\"\n    },\n    \"orderNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable order number\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Customer identifier in Plex\"\n    },\n    \"customerName\": {\n      \"type\": \"string\",\n      \"description\": \"Customer name\"\n    },\n    \"orderDate\": {\n      \"type\": \"string\",\n \
  \     \"format\": \"date\",\n      \"description\": \"Date the order was placed\"\n    },\n    \"dueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Requested delivery date\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"New\", \"Confirmed\", \"In Production\", \"Shipped\", \"Delivered\", \"Cancelled\"],\n      \"description\": \"Current order status\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"enum\": [\"Normal\", \"Rush\", \"Just-In-Sequence\"],\n      \"description\": \"Order fulfillment priority\"\n    },\n    \"orderLines\": {\n      \"type\": \"array\",\n      \"description\": \"Line items in the order\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"partNumber\", \"quantity\"],\n        \"properties\": {\n          \"lineNumber\": {\n            \"type\": \"integer\",\n            \"description\": \"Sequential line number\"\n          },\n          \"\
  partNumber\": {\n            \"type\": \"string\",\n            \"description\": \"Plex part number\"\n          },\n          \"partDescription\": {\n            \"type\": \"string\",\n            \"description\": \"Part description\"\n          },\n          \"quantity\": {\n            \"type\": \"number\",\n            \"description\": \"Ordered quantity\"\n          },\n          \"unitOfMeasure\": {\n            \"type\": \"string\",\n            \"description\": \"Unit of measure (e.g., EA, LB, KG)\"\n          },\n          \"unitPrice\": {\n            \"type\": \"number\",\n            \"description\": \"Price per unit\"\n          },\n          \"totalPrice\": {\n            \"type\": \"number\",\n            \"description\": \"Total line price\"\n          },\n          \"quantityShipped\": {\n            \"type\": \"number\",\n            \"description\": \"Quantity already shipped\"\n          }\n        }\n      }\n    },\n    \"shippingAddress\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Delivery address\",\n      \"properties\": {\n        \"name\": { \"type\": \"string\" },\n        \"address1\": { \"type\": \"string\" },\n        \"address2\": { \"type\": \"string\" },\n        \"city\": { \"type\": \"string\" },\n        \"state\": { \"type\": \"string\" },\n        \"postalCode\": { \"type\": \"string\" },\n        \"country\": { \"type\": \"string\" }\n      }\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Order notes or special instructions\"\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rockwell-automation/refs/heads/main/json-schema/rockwell-automation-plex-order-schema.json
tags:
- Industrial Automation
- Manufacturing
- PLC
- SCADA
- IIoT
title: Rockwell Automation Plex Customer Order
---
