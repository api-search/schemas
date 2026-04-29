---
description: A complete purchase order document representing a buyer's commitment to purchase goods or services from a supplier through the SAP Ariba Network
layout: schema
name: PurchaseOrder
properties_list:
- description: Unique purchase order identifier (UniqueName) including version
  name: orderId
  type: string
- description: ERP system purchase order number. Unique ID for every version of the purchase order in the backend ERP system.
  name: erpPONumber
  type: string
- description: Supplemental version number of the order. Incremented with each change request.
  name: versionNumber
  type: integer
- description: Date and time when the purchase order was created
  name: orderDate
  type: string
- description: Ordering method category indicating how the order was generated (e.g., manual, automatic, blanket release)
  name: orderMethodCategory
  type: string
- description: ISO 4217 currency code for the order
  name: currency
  type: string
- description: Purchasing organization identifier
  name: purchaseOrg
  type: string
- description: Purchasing group identifier
  name: purchaseGroup
  type: string
- description: Company code for the buying entity
  name: companyCode
  type: string
- description: Line items contained in the purchase order
  name: lineItems
  type: array
- description: Reference to the originating purchase requisition
  name: requisitionId
  type: string
- description: Reference to a master agreement or contract
  name: contractId
  type: string
- description: Header-level comments on the purchase order
  name: comments
  type: string
- description: Timestamp when the order was first created
  name: createdDate
  type: string
- description: Timestamp of the most recent modification
  name: lastModifiedDate
  type: string
- description: Timestamp when the order was closed
  name: closedDate
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-purchase-order-schema.json
slug: sap-ariba-procurement-purchase-order
source_filename: sap-ariba-procurement-purchase-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PurchaseOrder\",\n  \"type\": \"object\",\n  \"description\": \"A complete purchase order document representing a buyer's commitment to purchase goods or services from a supplier through the SAP Ariba Network\",\n  \"properties\": {\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique purchase order identifier (UniqueName) including version\"\n    },\n    \"erpPONumber\": {\n      \"type\": \"string\",\n      \"description\": \"ERP system purchase order number. Unique ID for every version of the purchase order in the backend ERP system.\"\n    },\n    \"versionNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Supplemental version number of the order. Incremented with each change request.\"\n    },\n    \"orderDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the purchase order was created\"\n    },\n    \"orderMethodCategory\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Ordering method category indicating how the order was generated (e.g., manual, automatic, blanket release)\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for the order\"\n    },\n    \"purchaseOrg\": {\n      \"type\": \"string\",\n      \"description\": \"Purchasing organization identifier\"\n    },\n    \"purchaseGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Purchasing group identifier\"\n    },\n    \"companyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Company code for the buying entity\"\n    },\n    \"lineItems\": {\n      \"type\": \"array\",\n      \"description\": \"Line items contained in the purchase order\"\n    },\n    \"requisitionId\": {\n      \"type\": \"string\",\n      \"description\": \"Reference to the originating purchase requisition\"\n    },\n    \"contractId\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Reference to a master agreement or contract\"\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"description\": \"Header-level comments on the purchase order\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the order was first created\"\n    },\n    \"lastModifiedDate\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of the most recent modification\"\n    },\n    \"closedDate\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the order was closed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-purchase-order-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: PurchaseOrder
---
