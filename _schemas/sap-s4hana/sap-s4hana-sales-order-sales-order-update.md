---
description: Request payload for updating sales order header fields
layout: schema
name: SalesOrderUpdate
properties_list:
- description: ''
  name: PurchaseOrderByCustomer
  type: string
- description: ''
  name: RequestedDeliveryDate
  type: string
- description: ''
  name: CustomerPaymentTerms
  type: string
- description: ''
  name: ShippingCondition
  type: string
- description: ''
  name: CompleteDeliveryIsDefined
  type: boolean
- description: ''
  name: HeaderBillingBlockReason
  type: string
- description: ''
  name: DeliveryBlockReason
  type: string
- description: ''
  name: IncotermsClassification
  type: string
- description: ''
  name: IncotermsTransferLocation
  type: string
- description: ''
  name: PricingDate
  type: string
- description: ''
  name: SDDocumentReason
  type: string
provider_name: SAP S/4HANA
provider_slug: sap-s4hana
schema_file: json-schema/sap-s4hana-sales-order-sales-order-update-schema.json
slug: sap-s4hana-sales-order-sales-order-update
source_filename: sap-s4hana-sales-order-sales-order-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrderUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Request payload for updating sales order header fields\",\n  \"properties\": {\n    \"PurchaseOrderByCustomer\": {\n      \"type\": \"string\"\n    },\n    \"RequestedDeliveryDate\": {\n      \"type\": \"string\"\n    },\n    \"CustomerPaymentTerms\": {\n      \"type\": \"string\"\n    },\n    \"ShippingCondition\": {\n      \"type\": \"string\"\n    },\n    \"CompleteDeliveryIsDefined\": {\n      \"type\": \"boolean\"\n    },\n    \"HeaderBillingBlockReason\": {\n      \"type\": \"string\"\n    },\n    \"DeliveryBlockReason\": {\n      \"type\": \"string\"\n    },\n    \"IncotermsClassification\": {\n      \"type\": \"string\"\n    },\n    \"IncotermsTransferLocation\": {\n      \"type\": \"string\"\n    },\n    \"PricingDate\": {\n      \"type\": \"string\"\n    },\n    \"SDDocumentReason\": {\n      \"type\": \"string\"\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/json-schema/sap-s4hana-sales-order-sales-order-update-schema.json
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
title: SalesOrderUpdate
---
