---
description: Request payload for creating a new sales order item
layout: schema
name: SalesOrderItemCreate
properties_list:
- description: Material number
  name: Material
  type: string
- description: Requested quantity
  name: RequestedQuantity
  type: string
- description: Unit of measure
  name: RequestedQuantityUnit
  type: string
- description: Plant
  name: Plant
  type: string
- description: Item category
  name: SalesOrderItemCategory
  type: string
- description: Item description
  name: SalesOrderItemText
  type: string
- description: Customer PO number at item level
  name: PurchaseOrderByCustomer
  type: string
- description: Pricing date
  name: PricingDate
  type: string
- description: Payment terms
  name: CustomerPaymentTerms
  type: string
- description: Customer material number
  name: MaterialByCustomer
  type: string
- description: Batch number
  name: Batch
  type: string
- description: Production plant
  name: ProductionPlant
  type: string
- description: Storage location
  name: StorageLocation
  type: string
- description: Delivery priority
  name: DeliveryPriority
  type: string
- description: Incoterms classification
  name: IncotermsClassification
  type: string
- description: Incoterms location
  name: IncotermsTransferLocation
  type: string
- description: Pricing elements (deep insert)
  name: to_PricingElement
  type: array
- description: Schedule lines (deep insert)
  name: to_ScheduleLine
  type: array
- description: Partners (deep insert)
  name: to_Partner
  type: array
- description: Text records (deep insert)
  name: to_Text
  type: array
provider_name: SAP S/4HANA
provider_slug: sap-s4hana
schema_file: json-schema/sap-s4hana-sales-order-sales-order-item-create-schema.json
slug: sap-s4hana-sales-order-sales-order-item-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrderItemCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request payload for creating a new sales order item\",\n  \"properties\": {\n    \"Material\": {\n      \"type\": \"string\",\n      \"description\": \"Material number\"\n    },\n    \"RequestedQuantity\": {\n      \"type\": \"string\",\n      \"description\": \"Requested quantity\"\n    },\n    \"RequestedQuantityUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measure\"\n    },\n    \"Plant\": {\n      \"type\": \"string\",\n      \"description\": \"Plant\"\n    },\n    \"SalesOrderItemCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Item category\"\n    },\n    \"SalesOrderItemText\": {\n      \"type\": \"string\",\n      \"description\": \"Item description\"\n    },\n    \"PurchaseOrderByCustomer\": {\n      \"type\": \"string\",\n      \"description\": \"Customer PO number\
  \ at item level\"\n    },\n    \"PricingDate\": {\n      \"type\": \"string\",\n      \"description\": \"Pricing date\"\n    },\n    \"CustomerPaymentTerms\": {\n      \"type\": \"string\",\n      \"description\": \"Payment terms\"\n    },\n    \"MaterialByCustomer\": {\n      \"type\": \"string\",\n      \"description\": \"Customer material number\"\n    },\n    \"Batch\": {\n      \"type\": \"string\",\n      \"description\": \"Batch number\"\n    },\n    \"ProductionPlant\": {\n      \"type\": \"string\",\n      \"description\": \"Production plant\"\n    },\n    \"StorageLocation\": {\n      \"type\": \"string\",\n      \"description\": \"Storage location\"\n    },\n    \"DeliveryPriority\": {\n      \"type\": \"string\",\n      \"description\": \"Delivery priority\"\n    },\n    \"IncotermsClassification\": {\n      \"type\": \"string\",\n      \"description\": \"Incoterms classification\"\n    },\n    \"IncotermsTransferLocation\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Incoterms location\"\n    },\n    \"to_PricingElement\": {\n      \"type\": \"array\",\n      \"description\": \"Pricing elements (deep insert)\"\n    },\n    \"to_ScheduleLine\": {\n      \"type\": \"array\",\n      \"description\": \"Schedule lines (deep insert)\"\n    },\n    \"to_Partner\": {\n      \"type\": \"array\",\n      \"description\": \"Partners (deep insert)\"\n    },\n    \"to_Text\": {\n      \"type\": \"array\",\n      \"description\": \"Text records (deep insert)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/json-schema/sap-s4hana-sales-order-sales-order-item-create-schema.json
tags:
- Business Applications
- Cloud
- Enterprise Resource Planning
- ERP
- Finance
- Human Resources
- Inventory
- Logistics
- Manufacturing
- Plant Maintenance
- Procurement
- S/4HANA
- Sales
- SAP
title: SalesOrderItemCreate
---
