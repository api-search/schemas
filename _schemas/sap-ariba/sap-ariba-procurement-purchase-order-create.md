---
description: Request body for creating a new purchase order
layout: schema
name: PurchaseOrderCreate
properties_list:
- description: ERP system purchase order number
  name: erpPONumber
  type: string
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Purchasing organization identifier
  name: purchaseOrg
  type: string
- description: Purchasing group identifier
  name: purchaseGroup
  type: string
- description: Company code
  name: companyCode
  type: string
- description: ''
  name: lineItems
  type: array
- description: Reference to originating requisition
  name: requisitionId
  type: string
- description: Reference to master agreement
  name: contractId
  type: string
- description: Header-level comments
  name: comments
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-purchase-order-create-schema.json
slug: sap-ariba-procurement-purchase-order-create
source_filename: sap-ariba-procurement-purchase-order-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PurchaseOrderCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new purchase order\",\n  \"properties\": {\n    \"erpPONumber\": {\n      \"type\": \"string\",\n      \"description\": \"ERP system purchase order number\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"purchaseOrg\": {\n      \"type\": \"string\",\n      \"description\": \"Purchasing organization identifier\"\n    },\n    \"purchaseGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Purchasing group identifier\"\n    },\n    \"companyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Company code\"\n    },\n    \"lineItems\": {\n      \"type\": \"array\"\n    },\n    \"requisitionId\": {\n      \"type\": \"string\",\n      \"description\": \"Reference to originating requisition\"\n    },\n\
  \    \"contractId\": {\n      \"type\": \"string\",\n      \"description\": \"Reference to master agreement\"\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"description\": \"Header-level comments\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-purchase-order-create-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: PurchaseOrderCreate
---
