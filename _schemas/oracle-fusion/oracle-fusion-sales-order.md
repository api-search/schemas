---
description: A sales order in Oracle Fusion Cloud SCM representing a customer order for products or services, managed through the Order Management module including order lines, fulfillment, and shipping details.
layout: schema
name: Oracle Fusion Cloud Sales Order
properties_list:
- description: Unique system-generated order identifier
  name: OrderId
  type: integer
- description: Order number visible to users
  name: OrderNumber
  type: string
- description: Order type classification
  name: OrderType
  type: string
- description: Customer name on the order
  name: CustomerName
  type: string
- description: Customer account number
  name: CustomerNumber
  type: string
- description: Business unit processing the order
  name: BusinessUnit
  type: string
- description: Date the order was placed
  name: OrderDate
  type: string
- description: Customer-requested shipping date
  name: RequestedShipDate
  type: string
- description: Total order amount
  name: TotalAmount
  type: number
- description: ISO 4217 currency code
  name: CurrencyCode
  type: string
- description: Current order status
  name: Status
  type: string
- description: Shipping destination address
  name: ShipToAddress
  type: string
- description: Billing address
  name: BillToAddress
  type: string
- description: Order line items
  name: OrderLines
  type: array
- description: Record creation timestamp
  name: CreationDate
  type: string
- description: Last modification timestamp
  name: LastUpdateDate
  type: string
provider_name: Oracle Fusion Cloud Applications
provider_slug: oracle-fusion
schema_file: json-schema/oracle-fusion-sales-order-schema.json
slug: oracle-fusion-sales-order
source_filename: oracle-fusion-sales-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/schemas/oracle-fusion/sales-order.json\",\n  \"title\": \"Oracle Fusion Cloud Sales Order\",\n  \"description\": \"A sales order in Oracle Fusion Cloud SCM representing a customer order for products or services, managed through the Order Management module including order lines, fulfillment, and shipping details.\",\n  \"type\": \"object\",\n  \"required\": [\"OrderType\", \"CustomerName\", \"BusinessUnit\"],\n  \"properties\": {\n    \"OrderId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique system-generated order identifier\"\n    },\n    \"OrderNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Order number visible to users\"\n    },\n    \"OrderType\": {\n      \"type\": \"string\",\n      \"description\": \"Order type classification\"\n    },\n    \"CustomerName\": {\n      \"type\": \"string\",\n      \"description\": \"Customer name\
  \ on the order\"\n    },\n    \"CustomerNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Customer account number\"\n    },\n    \"BusinessUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Business unit processing the order\"\n    },\n    \"OrderDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the order was placed\"\n    },\n    \"RequestedShipDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Customer-requested shipping date\"\n    },\n    \"TotalAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Total order amount\",\n      \"minimum\": 0\n    },\n    \"CurrencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Open\", \"Booked\", \"Closed\", \"Cancelled\", \"Awaiting Shipping\", \"Awaiting Billing\"\
  ],\n      \"description\": \"Current order status\"\n    },\n    \"ShipToAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Shipping destination address\"\n    },\n    \"BillToAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Billing address\"\n    },\n    \"OrderLines\": {\n      \"type\": \"array\",\n      \"description\": \"Order line items\",\n      \"items\": {\n        \"$ref\": \"#/$defs/OrderLine\"\n      }\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp\"\n    },\n    \"LastUpdateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\"\n    }\n  },\n  \"$defs\": {\n    \"OrderLine\": {\n      \"type\": \"object\",\n      \"description\": \"Individual line item on a sales order\",\n      \"properties\": {\n        \"LineId\": {\n          \"type\": \"integer\",\n          \"\
  description\": \"Order line identifier\"\n        },\n        \"LineNumber\": {\n          \"type\": \"integer\",\n          \"description\": \"Line number within the order\"\n        },\n        \"ItemNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Product item number\"\n        },\n        \"ItemDescription\": {\n          \"type\": \"string\",\n          \"description\": \"Product description\"\n        },\n        \"OrderedQuantity\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity ordered\",\n          \"minimum\": 0\n        },\n        \"UnitOfMeasure\": {\n          \"type\": \"string\",\n          \"description\": \"Unit of measure\"\n        },\n        \"UnitSellingPrice\": {\n          \"type\": \"number\",\n          \"description\": \"Selling price per unit\"\n        },\n        \"ExtendedAmount\": {\n          \"type\": \"number\",\n          \"description\": \"Total line amount (quantity times price)\"\n        },\n\
  \        \"RequestedShipDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Line-level requested ship date\"\n        },\n        \"Status\": {\n          \"type\": \"string\",\n          \"description\": \"Line status\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-fusion/refs/heads/main/json-schema/oracle-fusion-sales-order-schema.json
tags:
- Cloud
- CX
- Enterprise
- EPM
- ERP
- HCM
- Project Management
- REST API
- SaaS
- SCM
title: Oracle Fusion Cloud Sales Order
---
