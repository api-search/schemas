---
description: Schema for SAP S/4HANA Sales Order Item entity (A_SalesOrderItem) from the API_SALES_ORDER_SRV OData service. Represents a line item within a sales order including material, quantity, pricing, and status data.
layout: schema
name: SAP Sales Order Item
properties_list:
- description: Sales order number
  name: SalesOrder
  type: string
- description: Sales order item number
  name: SalesOrderItem
  type: string
- description: Sales document item category
  name: SalesOrderItemCategory
  type: string
- description: Short text for the sales order item
  name: SalesOrderItemText
  type: string
- description: Material number
  name: Material
  type: string
- description: Material number used by customer
  name: MaterialByCustomer
  type: string
- description: Cumulative order quantity in sales units
  name: RequestedQuantity
  type: string
- description: Sales unit
  name: RequestedQuantityUnit
  type: string
- description: Net value of the item in document currency
  name: NetAmount
  type: string
- description: SD document currency
  name: TransactionCurrency
  type: string
- description: Material group
  name: MaterialGroup
  type: string
- description: Batch number
  name: Batch
  type: string
- description: Plant (delivering)
  name: Plant
  type: string
- description: Storage location
  name: StorageLocation
  type: string
- description: Shipping point / receiving point
  name: ShippingPoint
  type: string
- description: Overall processing status of the item
  name: SDProcessStatus
  type: string
- description: Delivery status
  name: DeliveryStatus
  type: string
- description: Billing status
  name: OrderRelatedBillingStatus
  type: string
provider_name: SAP Sales and Distribution (SD)
provider_slug: sap-sales-and-distribution-sd
schema_file: json-schema/sap-sd-sales-order-item-schema.json
slug: sap-sd-sales-order-item
source_filename: sap-sd-sales-order-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap-sd-sales-order-item\",\n  \"title\": \"SAP Sales Order Item\",\n  \"description\": \"Schema for SAP S/4HANA Sales Order Item entity (A_SalesOrderItem) from the API_SALES_ORDER_SRV OData service. Represents a line item within a sales order including material, quantity, pricing, and status data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SalesOrder\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Sales order number\"\n    },\n    \"SalesOrderItem\": {\n      \"type\": \"string\",\n      \"maxLength\": 6,\n      \"description\": \"Sales order item number\"\n    },\n    \"SalesOrderItemCategory\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Sales document item category\"\n    },\n    \"SalesOrderItemText\": {\n      \"type\": \"string\",\n      \"maxLength\": 40,\n      \"description\"\
  : \"Short text for the sales order item\"\n    },\n    \"Material\": {\n      \"type\": \"string\",\n      \"maxLength\": 40,\n      \"description\": \"Material number\"\n    },\n    \"MaterialByCustomer\": {\n      \"type\": \"string\",\n      \"maxLength\": 35,\n      \"description\": \"Material number used by customer\"\n    },\n    \"RequestedQuantity\": {\n      \"type\": \"string\",\n      \"description\": \"Cumulative order quantity in sales units\"\n    },\n    \"RequestedQuantityUnit\": {\n      \"type\": \"string\",\n      \"maxLength\": 3,\n      \"description\": \"Sales unit\"\n    },\n    \"NetAmount\": {\n      \"type\": \"string\",\n      \"description\": \"Net value of the item in document currency\"\n    },\n    \"TransactionCurrency\": {\n      \"type\": \"string\",\n      \"maxLength\": 5,\n      \"description\": \"SD document currency\"\n    },\n    \"MaterialGroup\": {\n      \"type\": \"string\",\n      \"maxLength\": 9,\n      \"description\": \"Material group\"\n\
  \    },\n    \"Batch\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Batch number\"\n    },\n    \"Plant\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Plant (delivering)\"\n    },\n    \"StorageLocation\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Storage location\"\n    },\n    \"ShippingPoint\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Shipping point / receiving point\"\n    },\n    \"SDProcessStatus\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Overall processing status of the item\"\n    },\n    \"DeliveryStatus\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Delivery status\"\n    },\n    \"OrderRelatedBillingStatus\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Billing status\"\n    }\n  },\n  \"required\": [\"SalesOrder\"\
  , \"SalesOrderItem\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/json-schema/sap-sd-sales-order-item-schema.json
tags:
- Distribution
- ERP
- OData
- S/4HANA
- Sales
- SAP
title: SAP Sales Order Item
---
