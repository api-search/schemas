---
description: Request payload for updating sales order item fields
layout: schema
name: SalesOrderItemUpdate
properties_list:
- description: ''
  name: RequestedQuantity
  type: string
- description: ''
  name: RequestedQuantityUnit
  type: string
- description: ''
  name: Plant
  type: string
- description: ''
  name: SalesOrderItemText
  type: string
- description: ''
  name: PricingDate
  type: string
- description: ''
  name: CustomerPaymentTerms
  type: string
- description: ''
  name: ItemBillingBlockReason
  type: string
- description: ''
  name: SalesDocumentRjcnReason
  type: string
- description: ''
  name: DeliveryPriority
  type: string
- description: ''
  name: IncotermsClassification
  type: string
- description: ''
  name: IncotermsTransferLocation
  type: string
provider_name: SAP S/4HANA
provider_slug: sap-s4hana
schema_file: json-schema/sap-s4hana-sales-order-sales-order-item-update-schema.json
slug: sap-s4hana-sales-order-sales-order-item-update
source_filename: sap-s4hana-sales-order-sales-order-item-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrderItemUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Request payload for updating sales order item fields\",\n  \"properties\": {\n    \"RequestedQuantity\": {\n      \"type\": \"string\"\n    },\n    \"RequestedQuantityUnit\": {\n      \"type\": \"string\"\n    },\n    \"Plant\": {\n      \"type\": \"string\"\n    },\n    \"SalesOrderItemText\": {\n      \"type\": \"string\"\n    },\n    \"PricingDate\": {\n      \"type\": \"string\"\n    },\n    \"CustomerPaymentTerms\": {\n      \"type\": \"string\"\n    },\n    \"ItemBillingBlockReason\": {\n      \"type\": \"string\"\n    },\n    \"SalesDocumentRjcnReason\": {\n      \"type\": \"string\"\n    },\n    \"DeliveryPriority\": {\n      \"type\": \"string\"\n    },\n    \"IncotermsClassification\": {\n      \"type\": \"string\"\n    },\n    \"IncotermsTransferLocation\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/json-schema/sap-s4hana-sales-order-sales-order-item-update-schema.json
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
title: SalesOrderItemUpdate
---
