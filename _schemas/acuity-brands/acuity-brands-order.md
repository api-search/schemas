---
description: An Acuity Brands order with status and shipment information
layout: schema
name: Order
properties_list:
- description: Acuity Brands order number
  name: orderId
  type: string
- description: Distributor purchase order number
  name: purchaseOrderNumber
  type: string
- description: ''
  name: status
  type: string
- description: Date order was placed
  name: orderDate
  type: string
- description: Estimated ship date
  name: estimatedShipDate
  type: string
- description: Actual ship date
  name: actualShipDate
  type: string
- description: Order line items
  name: lineItems
  type: array
- description: Total order amount
  name: totalAmount
  type: number
- description: ''
  name: shipToAddress
  type: object
provider_name: acuity-brands
provider_slug: acuity-brands
schema_file: json-schema/acuity-brands-order-schema.json
slug: acuity-brands-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/acuity-brands/acuity-brands-order-schema.json\",\n  \"title\": \"Order\",\n  \"description\": \"An Acuity Brands order with status and shipment information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"Acuity Brands order number\",\n      \"example\": \"ACB-2026-001234\"\n    },\n    \"purchaseOrderNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Distributor purchase order number\",\n      \"example\": \"PO-55678\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"processing\",\n        \"shipped\",\n        \"delivered\",\n        \"cancelled\"\n      ],\n      \"example\": \"shipped\"\n    },\n    \"orderDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date order was placed\"\
  ,\n      \"example\": \"2026-04-15\"\n    },\n    \"estimatedShipDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Estimated ship date\",\n      \"example\": \"2026-04-20\"\n    },\n    \"actualShipDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Actual ship date\",\n      \"example\": \"2026-04-19\"\n    },\n    \"lineItems\": {\n      \"type\": \"array\",\n      \"description\": \"Order line items\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"lineNumber\": {\n            \"type\": \"integer\",\n            \"example\": 1\n          },\n          \"productNumber\": {\n            \"type\": \"string\",\n            \"example\": \"LBL4 48L ADP\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"example\": \"4FT LED Wrap Light\"\n          },\n          \"quantity\": {\n            \"type\": \"integer\",\n   \
  \         \"example\": 10\n          },\n          \"unitPrice\": {\n            \"type\": \"number\",\n            \"example\": 45.5\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"example\": \"shipped\"\n          }\n        }\n      }\n    },\n    \"totalAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Total order amount\",\n      \"example\": 455.0\n    },\n    \"shipToAddress\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"ABC Electrical Distributors\"\n        },\n        \"street\": {\n          \"type\": \"string\",\n          \"example\": \"123 Main St\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"example\": \"Atlanta\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"example\": \"GA\"\n        },\n        \"zip\": {\n          \"type\": \"string\",\n          \"example\"\
  : \"30301\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acuity-brands/refs/heads/main/json-schema/acuity-brands-order-schema.json
tags: []
title: Order
---
